![Logo](docs/resources/logo/logo-64.png)

# react-simple-wysiwyg
[![Build Status](https://travis-ci.org/megahertz/react-simple-wysiwyg.svg?branch=master)](https://travis-ci.org/megahertz/react-simple-wysiwyg)
[![NPM version](https://badge.fury.io/js/react-simple-wysiwyg.svg)](https://badge.fury.io/js/react-simple-wysiwyg)
[![Dependencies status](https://david-dm.org/megahertz/react-simple-wysiwyg/status.svg)](https://david-dm.org/megahertz/react-simple-wysiwyg)
[![npm bundle size](https://img.shields.io/bundlephobia/minzip/react-simple-wysiwyg.svg?color=rgb%2868%2C%20204%2C%2017%29)](https://bundlephobia.com/result?p=react-simple-wysiwyg@0.0.3)

Simple and lightweight React WYSIWYG editor. [Demo](https://megahertz.github.io/react-simple-wysiwyg/)

[![Screenshot](docs/resources/screenshot.png)](https://megahertz.github.io/react-simple-wysiwyg/)

## Description

**The project is in alpha stage.**

It can be helpful if you only need basic text operations

 - Pretty small (~10kb, ~4kb gzipped)
 - Simple to configure
 - Simple to extend

Of course, it's not so powerful as other complex editors. It DOES NOT:

 - ✗ change HTML generated by browser (sometimes it can too dirty)
 - ✗ sanitize HTML (you can use [sanitize-html](https://www.npmjs.com/package/sanitize-html))
 - ✗ contain a lot of complex feature as others (like table editor, image editor and so on)
 - ✗ support old browser

If you need more powerful solution for React, you'd better take a look at:

 - [draft.js](https://draftjs.org/) or draft-powered editor like
   [react-rte](https://github.com/sstur/react-rte)
 - classic solution like [CKEditor](https://ckeditor.com/) and
   (TinyMCE)[https://www.tiny.cloud/]
 - [Quill](https://github.com/zenoamaro/react-quill) and
   [Summernote](https://github.com/summernote/react-summernote)


## Usage

 1. Install with [npm](https://npmjs.org/package/react-simple-wysiwyg):

    `npm install react-simple-wysiwyg`
    
    or [CDN (unpkg.com)](https://unpkg.com/react-simple-wysiwyg@0.0.3/)
   
    `<script src="//unpkg.com/react-simple-wysiwyg"></script>`
    
 2. Use it you React component
 
    ```jsx
    import { DefaultEditor } from 'react-simple-wysiwyg';
    
    function App() {
      const [html, setHtml] = React.useState('my <b>HTML</b>');
      
      const onChange = (e) => {
        setHtml(e.target.value);
      };
    
      return (
        <DefaultEditor value={html} onChange={onChange} />
      );
    }
    ```
  
## Credits

 - Based on 
   [lovasoa/react-contenteditable](https://github.com/lovasoa/react-contenteditable)
 - Uses [Material Design Icons](http://materialdesignicons.com/)
