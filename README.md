## Clone the project

- git clone https://github.com/gmerialdo/Laravelapp.git

## Go into repository, create .env and run app through Docker

- cd Laravelapp
- cp .env.example .env
- docker run --rm -v $(pwd):/Laravelapp composer/composer install
- sail up -d

## Run the migrations etc. 
- sail artisan migrate
- sail artisan key:generate
- sail npm install
- npm run dev
