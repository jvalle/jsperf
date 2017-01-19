---
title: string compare vs string methods
setup: |
  var strings = [
    'hello',
    'party',
    'good_time',
    'internet'
  ];
tests:
  -
    name: string compare
    code: |
      var i = Math.round(Math.random() * 4);
      
      strings[i] === 'good_time' ? 'good time' : strings[i];
  -
    name: string methods
    code: |
      var i = Math.round(Math.random() * 4);
      
      strings[i].split('_').join(' ');
---
string compare vs method calls
