# RiskCog
## Unobtrusive and Continuous User Identification on Smartphones in the Wild

Report : [Currently unavailable(being reviewed)](https://github.com/NathanShi)

Download link : [Currently unavailable(demoing to Alibaba)](https://github.com/NathanShi)

Our App manual : 
- [SensorDemo App manual](https://drive.google.com/file/d/0B9GDDA3vZuKZbVdBTnMzZnF1NXc/view?usp=sharing)

---

### Bug Fixed Log

- **Empty Password:** Add function in `nConfirmButtonClick()` in `PasswordActivity.java`.

- **Vertical Screen Overlapped Button and Text:**  Add `android:screenOrientation="portrait"` in `AndroidManifest.xml`.

- **Wrong "back" button function in password changing:** Change function `onConfirmButtonClick()` in `PasswordActivity.java`.

- **No reminders of phones that sensors not working:** Add `dialog` in `CollectDataService.java` for reminder.

- **"Suspicious User" dialogs pop up simultaneously:** Add `isCurrentPopupFinish` variable in `LongService.java` function `onStartCommand()`.

- **"Suspicious User" dialogs not sequential** Add two more variables in `CustomizedDialog.java` and `CollectDataService.java` to make user able to go back to previous dialog to change selections.

- **In dialogs user cannot change the service pause time** Add functions in `CollectDataService.java`.

- **After changing the password, the service back to 'Ready':** Change function `startPasswordSetting()` in `MainActivity.java` to remain the state.

- **Walk data was assigned to sit model:** Fixed on server side by teammates.

- **Abnormal data added to model:** Add if-else in function `writeTxt()` in `CollectDataService.java` to filter these data.

- **No time reminder for "Suspicious User" dialog:** Add variables to get timestamp of the return result in `DetectService.java`

- **New Interface and Icon**

- **Five times false alarm will return to training phase:** Add variables and functions to `DetectService.java`

- **One model exist will also generate dialog if accuracy is low:** Add this function from server side and client side.
  
 
