
### Angular is already using ng-template under the hood in many of the structural directives that we use all the time: ngIf, ngFor and ngSwitch.

in ts file
    loginText = 'Login';
    signUpText = 'Sign Up'; 
    lessons = ['Lesson 1', 'Lessons 2'];

      <ng-template [ngIf]="lessons" [ngIfElse]="loading">
       <div class="lesson" *ngFor="let lesson of lessons">
            <div class="lesson-detail">
                {{lesson | json}}
            </div>
        </div>
     </ng-template>
	 
     <div *ngIf="lessons">
        <div class="lesson" *ngFor="let lesson of lessons">
            <div class="lesson-detail">
                {{lesson | json}}
            </div>
        </div>
    </div>
     
	 <ng-template #loading>
          <div>Loading...</div>
      </ng-template>