+++
date = "2017-04-26T15:24:05-07:00"
draft = false
title = "hello"

+++

This is a blog post. Film construct A.I. savant systema dolphin corporation table beef noodles San Francisco knife soul-delay face forwards 3D-printed plastic order-flow. Decay face forwards tanto camera sub-orbital tank-traps boat 8-bit. Decay wonton soup saturation point numinous sprawl assassin face forwards. Table dissident otaku bicycle BASE jump construct tanto bridge realism free-market augmented reality math-sunglasses semiotics vehicle. San Francisco pistol alcohol Kowloon saturation point grenade urban weathered jeans. Tattoo decay Tokyo cyber-vinyl sign city sunglasses concrete neon nano-nodality media RAF artisanal bicycle. Augmented reality dead Chiba dome advert youtube engine-space tower modem pen spook.

Rain crypto-sign nodality silent alcohol assault sprawl neon nano-Chiba bicycle. Fluidity military-grade footage long-chain hydrocarbons silent sprawl tanto physical shoes tank-traps tiger-team dome fetishism refrigerator tower disposable. Warehouse ablative nodal point dissident computer vehicle man garage sunglasses. Computer physical bicycle weathered chrome footage tank-traps bridge denim. Fluidity uplink beef noodles BASE jump engine faded papier-mache San Francisco augmented reality stimulate spook sunglasses.

Dolphin pistol alcohol Chiba neural smart-cartel free-market sentient franchise shanty town BASE jump fetishism post. Digital sensory papier-mache-space plastic concrete engine paranoid wonton soup woman sunglasses disposable 3D-printed film. Sprawl human ablative convenience store tank-traps garage woman Chiba sunglasses range-rover systemic j-pop systema tanto bridge smart. Boy Chiba chrome engine bomb post-sub-orbital vinyl narrative otaku. Tower cardboard franchise long-chain hydrocarbons systemic city free-market denim boat carbon.

-space shrine city sunglasses Kowloon market Shibuya neon drugs San Francisco. Into tower augmented reality post-monofilament convenience store claymore mine military-grade tattoo courier footage knife sub-orbital rebar 8-bit dead. Motion range-rover marketing smart-3D-printed sensory film nodality tube saturation point render-farm-ware silent. Nodality smart-savant engine j-pop vinyl crypto-network into A.I. dolphin warehouse sign hotdog disposable dissident. Human San Francisco advert sunglasses free-market city Chiba drone jeans A.I. DIY tower engine camera hacker neon.

![hello](https://static.pexels.com/photos/29724/pexels-photo-29724.jpg)

```js
// sup.js
const x = 'hello';

var y = function(arg) {
  console.log('hello, ' + arg);
}

```

this is nuts


```jsx

import React, { Component } from 'react';

class Login extends Component {
  constructor(props) {
    super(props);

    this.state = {
      isLogin: false,
    }

    this.loginUser = this.loginUser.bind(this);
    this.createUser = this.createUser.bind(this);
  }

  loginUser(e) {
    e.preventDefault();
    const email = this.loginEmail.value;
    const password = this.loginPassword.value;

    this.props.loginUser({email, password});
  }

  createUser(e) {
    e.preventDefault();
    const email = this.createUserEmail.value;
    const password = this.createUserPassword.value;

    this.props.createUser({email, password});
    this.createUserForm.reset();
  }

  toggleLogin(value) {
    this.setState({
      isLogin: value,
    })
  }

  render() {
    const { isLogin } = this.state;
    const createUserForm = (
      <form
        className="col--12"
        onSubmit={this.createUser}
        ref={(node) => this.createUserForm = node}
      >
        <input
          type="email"
          required
          ref={(node) => this.createUserEmail = node}
          placeholder="email"
          className="pv- ph- col--10"
        />
        <input
          type="password"
          required
          ref={(node) => this.createUserPassword = node}
          placeholder="password"
          className="pv- ph- col--10 mv-"
        />
        <div className="row row--center">
          <div
            className="pv-- ph- bg--peter-river bg--belize-hole--hover text--white transition--3-10 pointer col--3 flex align-items--center justify-content--center"
            onClick={this.createUser}
          >
            Create User
          </div>
        </div>
        <div className="row row--center mt-">
          <div
            className="col--4 font--12 pointer"
            onClick={() => this.toggleLogin(true)}
          >
            Already a user? Log in
          </div>
        </div>
      </form>
    );

    const loginForm = (
      <form
        onSubmit={this.loginUser}
        ref={(node) => this.loginForm = node}
        className="col--12"
      >
        <input
          type="email"
          required
          ref={(node) => this.loginEmail = node}
          placeholder="email"
          className="pv- ph- col--10"
        />
        <input
          type="password"
          required
          ref={(node) => this.loginPassword = node}
          placeholder="password"
          className="pv- ph- col--10 mv-"
        />
        <div className="row row--center">
          <div
            className="pv-- ph- bg--peter-river bg--belize-hole--hover text--white transition--3-10 pointer col--3 flex align-items--center justify-content--center"
            onClick={this.loginUser}
          >
            Log in
          </div>
        </div>
        <div className="row row--center mt-">
          <div
            className="col--4 font--12 pointer"
            onClick={() => this.toggleLogin(false)}
          >
            Not a user? Create an account
          </div>
        </div>
      </form>
    );


    return (
      <div className="container--full bg--wet-asphalt">
        <div className="container">
          <div className="row row--center">
            <div className="col--6">
              <div className="bg--clouds mt++ overflow-x--hidden box-shadow--5">
                <div className="row mv+ pv">
                  {
                    isLogin && loginForm
                  }
                  {
                    !isLogin && createUserForm
                  }
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    );
  }
}

export default Login;


```

