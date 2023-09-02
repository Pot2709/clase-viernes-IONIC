# clase-viernes-IONIC



page.ts es para escribir los codigos

import { HttpClient } from '@angular/common/http';

   news : any = [];

    constructor(private http : HttpClient) {
    this.http.get<any>('assets/noticias.json')
    .subscribe(data => {
      console.log('news', data);
      this.news = data.articles;
    }
      )
  }

}





