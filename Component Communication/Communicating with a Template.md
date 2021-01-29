# Communicating with a Template

## Notifying the component of User Changes and perfome an action: 
For this, we can use two-way binding

in the .ts:

    unFiltre : string;

    onFilterCHange(leFilter: string): void{
        //because we no loger using two-way binding [()]
        this.unFiltre = leFiltre;

        //performe chanegs
    }



in the template :

    <input type='text' [ngModel]='unFiltre'
                       (ngModelChange='onFilterCHange($event)') />