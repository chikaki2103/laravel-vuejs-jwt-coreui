# Laravel 5.6 + CoreUI Admin Bootstrap + VueJS + JWT


## What is this?

This is a boilerplate for a SPA Admin application with Laravel 5.6, VueJS, CoreUI and JWT authentication (hope it can save up some time for someone who's developing a project like that).
It's using following open sources:
- [laravel-coreui-vue](https://github.com/Braunson/laravel-coreui-vue)
- [tymon/jwt-auth](https://github.com/tymondesigns/jwt-auth)
- [websanova/vue-auth](https://github.com/websanova/vue-auth)


## What have been implemented:

- integrated Laravel 5.6 with [tymon/jwt-auth](https://github.com/tymondesigns/jwt-auth). There are some small problems when integrate with this library, so I have used the branch 'develop'.
- integrated [websanova/vue-auth](https://github.com/websanova/vue-auth) with the current [laravel-coreui-vue](https://github.com/Braunson/laravel-coreui-vue), now it can authenticate users from Laravel backend, and authorize on each Vue routes.
- upgrade BootstrapVue to the latest version, fixed some issues during migration.


## Getting Started

```
composer install
cp .env.example .env
php artisan key:generate
php artisan jwt:secret
php artisan migrate:refresh --seed
npm install
npm run dev
php artisan serve

```
### Testing users:
- admin@test.com / 123456
- moderator@test.com / 123456
- user@test.com /123456


## License

The MIT License (MIT)
