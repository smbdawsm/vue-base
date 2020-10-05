<template>
<div>
 <div>
        <div class="header-dark">
            <nav class="navbar navbar-dark navbar-expand-lg navigation-clean-search">
                <div class="container"><a class="navbar-brand" href="#">Otelit Rent Base</a><button data-toggle="collapse" class="navbar-toggler" data-target="#navcol-1"><span class="sr-only">Toggle navigation</span><span class="navbar-toggler-icon"></span></button>
                    <div class="collapse navbar-collapse"
                        id="navcol-1">
                        <ul class="nav navbar-nav">
                            <li class="nav-item"><a class="nav-link" href="/objects">Объекты</a></li>
                        </ul>
                        <form class="form-inline mr-auto" target="_self">
                            <div class="form-group"><label for="search-field"><i class="fa fa-search"></i></label><input class="form-control search-field" type="search" id="search-field" name="search" v-on:keyup.enter="search"></div>
                        </form><span class="navbar-text"></span></div>
                </div>
            </nav>
        </div>
    </div>
    <div >
        <router-view />
    </div>
    
</div>
</template>