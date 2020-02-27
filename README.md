#### 1. Clone/Download this project
`$ git clone https://github.com/rckycls/laravel-passport-template.git`

#### 2. Go to the project directory and install packages
`$ composer install`

#### 3. Copy .env.example as .env and fill it with your env data
`$ cp .env.example .env`

#### 4. Migrate database
`$ php artisan migrate`

#### 5. Install passport
`$ php artisan passport:install`

#### 6. Start the project and start modifying the controllers and routes
`$ php artisan serve`

`$ php -S localhost:8000 -t public` *// if you cannot run the above code*

----

## How to get access token
    $response = $http->post('http://your-app.com/oauth/token', [
        'form_params' => [
            'grant_type' => 'authorization_code',
            'client_id' => 'client-id',
            'client_secret' => 'client-secret',
            'redirect_uri' => 'http://example.com/callback',
            'code' => $request->code,
        ],
    ]);
