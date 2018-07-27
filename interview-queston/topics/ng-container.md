### ng-container directive
### In order to avoid having to create that extra div, 
we can use ng-container directive:

in ts file
    loginText = 'Login';
    signUpText = 'Sign Up'; 
    lessons = ['Lesson 1', 'Lessons 2'];

in htmls
    <ng-container *ngIf="lessons">
        <div class="lesson" *ngFor="let lesson of lessons">
            <div class="lesson-detail">
                {{lesson | json}}
            </div>
        </div>
    </ng-container>

### Dynamic Template Creation with the ngTemplateOutlet directive
the template itself and instantiate it anywhere on the page, using the ngTemplateOutlet directive:

<ng-container *ngTemplateOutlet="loading"></ng-container>