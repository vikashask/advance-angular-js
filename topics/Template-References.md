    @Component({
    selector: 'app-root',
    template: `      
        <ng-template #defaultTabButtons>
            <button class="tab-button" (click)="login()">
                {{loginText}}
            </button>
            <button class="tab-button" (click)="signUp()">
                {{signUpText}}
            </button>
        </ng-template>
    `})
    export class AppComponent implements OnInit {

        @ViewChild('defaultTabButtons')
        private defaultTabButtonsTpl: TemplateRef<any>;

        ngOnInit() {
            console.log(this.defaultTabButtonsTpl);
        }

    }

-DOM element or component, by providing the template reference name defaultTabButtons to the ViewChild decorator.


