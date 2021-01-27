## mat table
Data should be passed as a DataSource

### exemple: 

in the .ts file 

    //Type of data we want to show
    notes: Note[];
    
    // exemple of attribute of type notes
    displayedColumns: string[] = ['position', 'title', 'date' ];
    dataSource: MatTableDataSource<Note>;

    ngOnInit(): void {
      this.dataSource = new MatTableDataSource<Note>(this.notes);
  }
