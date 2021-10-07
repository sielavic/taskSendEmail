
string mailTo = Get<string>("ProcessSchemaEmail");
string usrMessage = Get<string>("ProcessSchemaMail");


MailMessage mail = new MailMessage();
mail.From = new MailAddress(mailTo);//от кого dfjshhkgs@mail.ru
mail.To.Add(new MailAddress(mailTo)); // кому отправляем
mail.Subject = "Создана транзакция";
mail.Body = usrMessage;

SmtpClient client = new SmtpClient();
client.Host = "smtp.mail.ru";
client.Port = 2525;//Explicit SSL использует порты 25
client.EnableSsl = true;
client.Credentials = new NetworkCredential("dfjshhkgs@mail.ru", "");
client.DeliveryMethod = SmtpDeliveryMethod.Network;
client.Send(mail);
mail.Dispose();



return true;
