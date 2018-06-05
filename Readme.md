# Object rest

    const myObject = {
      lorem : 'ipsum',
      dolor : 'sit',
      amet : 'foo',
      bar : 'baz'
    };

    const { lorem, dolor, ...others } = myObject;

    // lorem === 'ipsum'
    // dolor === 'sit'
    // others === { amet : 'foo', bar : 'baz' }

# Object spread

    const obj1 = {
      amet : 'foo',
      bar : 'baz'
    };

    // đối với code sử dụng ES7
    const myObject = {
      lorem : 'ipsum',
      dolor : 'sit',
      ...obj1  
    };

    // đối với code sử dụng ES6
    const myObject = Object.assign({
      lorem : 'ipsum',
      dolor : 'sit'
    }, obj1);
    
    /*
    myObject === {
      lorem : 'ipsum',
      dolor : 'sit',
      amet : 'foo',
      bar : 'baz'
    };
    */