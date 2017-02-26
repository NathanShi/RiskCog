# RiskCog
## Unobtrusive and Continuous User Identification on Smartphones in the Wild

Led by Prof.Yan Chen and his phD student Zhengyang Qu in group of 9

Report : [Currently the paper is under reviewing](https://github.com/NathanShi)

Download link : [Currently unavailable(demoing to Alibaba)](https://github.com/NathanShi)

Our App manual : 
- [SensorDemo App manual(Chinese version)](https://drive.google.com/file/d/0B9GDDA3vZuKZaEFHRG5sU3h4Z3M/view?usp=sharing)

---
### Test Result

#### First round:

This time the required file number of sit and walk model is both 10. After training the accuracy is approximately 60% false detecting owner himself as "Suspicious User", which is not as expected since it will hurt user experience much. For successfully detecting other user as "Suspicious User" is approximately 80%, which is a good result yet still needs improvements.

#### Second round:

This time we changed the required file amount to 100, 10 times than last round. And right now the false alarm drops to 5%(60% before). Also, the dialog will allow user to set such false alarm data add into his model so that the current model will keep modify itself to be more accurate And the accuracy of successfully detecting other user as "Suspicious User" is 100%. It's more sensitive than last round.

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

- **Too many walk data was assigned to sit model:** Fixed on server side by teammates.

- **New Interface and Icon**
  
 
