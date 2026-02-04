# TODO: Integrate JWT Authentication and Authorization

## Steps to Complete

- [ ] Update user model to include hashed_password field (app/models/user.py)
- [ ] Add password to UserCreate schema, create UserLogin and Token schemas (app/schemas/user.py)
- [ ] Add JWT settings (SECRET_KEY, ALGORITHM, ACCESS_TOKEN_EXPIRE_MINUTES) to config (app/core/config.py)
- [ ] Add InvalidCredentialsException to exceptions (app/core/exceptions.py)
- [ ] Update repository: Add get_user_by_email, modify create_user to hash password (app/repositories/user_repo.py)
- [ ] Update service: Add register_user, authenticate_user, create_access_token functions (app/services/user_service.py)
- [ ] Update API: Add register and login endpoints, add JWT dependency for protected routes (app/api/user.py)
- [ ] Update main.py: Include auth router (app/main.py)
- [ ] Install dependencies: python-jose[cryptography], passlib[bcrypt]
- [ ] Test registration, login, and protected endpoints
