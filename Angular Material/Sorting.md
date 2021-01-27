## Sorting Columns

1- Add matSort in the <table> tag </br>
2- Add mat-sort-header in the <th> tag for the element we want to sort

3- in the Ts we add :

        @ViewChild(MatSort) sort: MatSort;

        ngAfterViewInit() {
            this.dataSource.sort = this.sort;
        }