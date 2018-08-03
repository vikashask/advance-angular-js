
    @Component({
    selector: 'app-root',
    template: `      

    <ng-template #estimateTemplate let-lessonsCounter="estimate">
        <div> Approximately {{lessonsCounter}} lessons ...</div>
    </ng-template>

    <ng-container 
    *ngTemplateOutlet="estimateTemplate;context:ctx">
    </ng-container>
    `})
    export class AppComponent {

        totalEstimate = 10;
        ctx = {estimate: this.totalEstimate};
    
    }
### o/p Approximately 10 lessons ...

>the input variable is called lessonsCounter, and it's defined via a ng-template property using the prefix let-

>The variable lessonsCounter is visible inside the ng-template body, but not outside

>That expression is evaluated against a context object, passed to ngTemplateOutlet together with the template to instantiate

>This context object must then have a property named estimate, for any value to be displayed inside the template

>the context object is passed to ngTemplateOutlet via the context property, that can receive any expression that evaluates to an object


