
 public isScreenSmall: boolean;

  constructor(private breakPoint: BreakpointObserver) { }

  ngOnInit(): void {
    this.breakPoint.observe([Breakpoints.Small, Breakpoints.XSmall])
    .subscribe((state: BreakpointState) => {
      //set isScreenSmall attribute to true if the screen is small
      this.isScreenSmall = state.matches;
    })