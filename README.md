<div align='center'>
  
# 💫 About Me:

🌱 Welcome I'm Delphine 🌱
<br><br>
🔭 I'm currently working on PHP, SQL and LARAVEL 🔭

# <img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/git%20repository.png" alt="Repository" height="30" width="30" /> Some repositories for various languages




<br>

| <img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/ArticleSelected.jpeg" height="250px" width="150px;"/><br /><sub><b>[Modèle-Vue-Contrôleur ](https://github.com/DelphineLecorney/mvc/blob/main/README.md)</b></sub> | <img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/Form.jpg" height="250px" width="150px;"/><br /><sub><b>[Hackers Poulette](https://github.com/DelphineLecorney/hackers-poulette)</b></sub> | <img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/Collection.JPG" height="250px" width="150px;"/><br /><sub><b>[Collection](https://github.com/DelphineLecorney/Collection)</b></sub> | <img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/Wahck-A-Mole.jpg" height="250px" width="150px;"/><br /><sub><b>[Whack A Mole](https://github.com/DelphineLecorney/Whack-A-Mole)</b></sub> |
| :---: | :---: | :---: | :---: |



<br>




[Tradding app](https://github.com/DelphineLecorney/TraddingApp)
</div>

```php
class AuthController extends Controller
{
    public function __construct()
    {
        $this->middleware('auth:api', ['except' => ['login', 'signup']]);
    }

    public function login(Request $request)
    {
        $request->validate([
            'email' => 'required|string|email',
            'password' => 'required|string',
        ]);

        $credentials = $request->only('email', 'password');
        if (!$token = JWTAuth::attempt($credentials)) {
            return response()->json(['message' => 'Unauthorized'],401);
        }

        $user = Auth::user();
        return response()->json([
            'user' => $user,
            'authorization' => [
                'token' => $token,
                'type' => 'bearer',
            ]
            ]);
    }
}
```

<br>

# <img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/Stacks_Logo.png" alt="Stacks" height="40" width="40" /> Tech Stacks :

<p align='left'>
  

<img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/html.png" alt="html5" height="60" width="60" /> 

<img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/CSS3.jpg" alt="css" height="60" width="60" /> 

<img src="https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/php.jpg" alt="PHP" height="60" width="60" /> 

![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)![SASS](https://img.shields.io/badge/SASS-hotpink.svg?style=flat&logo=SASS&logoColor=white)![LARAVEL](https://github.com/DelphineLecorney/DelphineLecorney/blob/main/images/Laravel.JPG)

<br>

# 📊 GitHub Stats:

![](https://github-readme-streak-stats.herokuapp.com/?user=DelphineLecorney&theme=dark&hide_border=false)

<br>

### 🔝 Top Contributed Repo
![](https://github-contributor-stats.vercel.app/api?username=DelphineLecorney&limit=5&theme=dark&combine_all_yearly_contributions=true)
</p>


## 🌐 Social 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B6.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/https://www.linkedin.com/in/delphine-lecorney-539781242/) 

<div class="badge-base LI-profile-badge" data-locale="fr_FR" data-size="medium" data-theme="dark" data-type="VERTICAL" data-vanity="delphine-lecorney" data-version="v1"><a class="badge-base__link LI-simple-link" href="https://be.linkedin.com/in/delphine-lecorney?trk=profile-badge">Delphine Lecorney</a></div>
              
---
[![](https://visitcount.itsvg.in/api?id=DelphineLecorney&icon=0&color=0)](https://visitcount.itsvg.in)
