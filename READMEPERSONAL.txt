      Nuovo progetto con

      npx nuxi init <PROJECT-NAME>
      cd <PROJECT-NAME>

      Poi

      npm install-yarn install per node modules / dependencies

      A questo punto il progetto è pronto per essere avviato con

      npm run dev


      TAILWIND 

      Per installare tailwind anzitutto digitare il comando 

      npm install --save-dev @nuxtjs/tailwindcss

      lo vedremo apparire nelle dependencies, poi digitare 

      npx tailwindcss init -p

      Così creeremo un file di confifurazione che necessiterà di alcune modifiche. Tra le parentesi della proprietà "content"
      aggiungeremo le route per tutti i file contenuti nel nostro progetto che necessitano di Vue ( Esempio - content : ["./**/*/.vue] )

      Per finire dovremo solo aggiungere 

      modules: ['@nuxtjs/tailwindcss'],

      nel file 
      
      nuxt.config.ts

      poi, dentro la cartella principale del progetto creare una cartella assets, che conterrà una cartella css che a sua volta conterrà un file

      tailwind.css

      questo file dovrà avere queste tre righe al suo interno

      @import 'tailwindcss/base';
      @import 'tailwindcss/components';
      @import 'tailwindcss/utilities';

      che ci permetteranno di utilizzare le classi di tailwind

      Ora dovremo solo importare questo file css nella nostra app, così

      import "./assets/css/tailwind.css

      --FINE--

