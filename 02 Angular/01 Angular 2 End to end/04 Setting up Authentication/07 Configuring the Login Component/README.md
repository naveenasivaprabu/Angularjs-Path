# 07 Angular 2 End to end - Setting up Authentication - Configuring the Login Component

- Login component same like as  signup component.
- Import user service and router

```javascript
import {UserService} from '../adminShared/user.service';
import { Router } from '@angular/router';
```
- based on function call the components and routers

```javascript
export class LoginComponent {
  email: string;
  password1: string;
  constructor(private userSVC: UserService, private router: Router){}

  login(){
    this.userSVC.login(this.email, this.password1);
    this.userSVC.verifyUser();
  }

  signup(){
    this.router.navigate(['/admin/signup']);
  }

  cancel(){
    this.router.navigate(['']);
  }

}
```