# RiskCog
## Unobtrusive and Continuous User Identification on Smartphones in the Wild

Led by Prof.Yan Chen and his phD student Zhengyang Qu in group of 9

Download link : [Currently unavailable(demo to Ali)]()

Our App manual : [SensorDemo App manual]()

### Bug Fixed Log

- **Empty Password**: In *PasswordActivity*: function *nConfirmButtonClick()* line 55 & 75 add two if... else... to check if the password is empty. 
  ~~~~
  line 55 : 
  if(SecondInput.getText().toString().equals("") || ThirdInput.getText().toString().equals(""))
  CustomizedDialog.createSimpleDialog(this, "Error", "Empty Input Password", false);
  else {...}
  ~~~~
  ~~~~
  line 73 :
  if (FirstInput.getText().toString().equals("") || SecondInput.getText().toString().equals(""))
  CustomizedDialog.createSimpleDialog(this, "Error", "Empty Input Password", false);
  else {...}
  ~~~~

