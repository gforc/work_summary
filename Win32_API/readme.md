
# what is win32_API
python can control the applicantions by win32_API

# instal
```
pip3.exe install pypiwin32
```

# example
## send email by outlook
```
import win32com.client as win32
# control outlook by the method 'Dispatch'
outlook = win32.Dispatch('outlook.application')
mail = outlook.CreateItem(0)
#receivers = ['name1@126.com; name2@126.com']
receivers = ['name1@126.com']
mail.To = receivers[0]
mail.Subject = 'test1'
mail.Body='aaaaaaaaaaaa'

#mail.Subject = sub.decode('utf-8')  
#mail.Body = body.decode('utf-8')  
# 添加附件  
# mail.Attachments.Add('D:\Users\xxx\Desktop\email.log')  
    
mail.Send()
```
