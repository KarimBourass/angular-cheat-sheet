## Pagination

1- Add in the html <b>outside</b> the table tag 

      <mat-paginator [pageSize]="5" [pageSizeOptions]="[5, 10, 20]" showFirstLastButtons></mat-paginator>

2- in the .ts file

    // import ViewChild and MatPaginator
    @ViewChild(MatPaginator) paginator: MatPaginator;

    //implements after view init
    ngAfterViewInit() {
      this.dataSource.paginator = this.paginator;
    }