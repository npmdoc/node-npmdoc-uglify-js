# api documentation for  [uglify-js (v2.8.16)](http://lisperator.net/uglifyjs)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-uglify-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-uglify-js)
#### JavaScript parser, mangler/compressor and beautifier toolkit

[![NPM](https://nodei.co/npm/uglify-js.png?downloads=true)](https://www.npmjs.com/package/uglify-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-uglify-js/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-uglify_js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-uglify-js/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-uglify-js/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Mihai Bazon",
        "email": "mihai.bazon@gmail.com",
        "url": "http://lisperator.net/"
    },
    "bin": {
        "uglifyjs": "bin/uglifyjs"
    },
    "browserify": {
        "transform": [
            "uglify-to-browserify"
        ]
    },
    "bugs": {
        "url": "https://github.com/mishoo/UglifyJS2/issues"
    },
    "dependencies": {
        "source-map": "~0.5.1",
        "uglify-to-browserify": "~1.0.0",
        "yargs": "~3.10.0"
    },
    "description": "JavaScript parser, mangler/compressor and beautifier toolkit",
    "devDependencies": {
        "acorn": "~0.6.0",
        "escodegen": "~1.3.3",
        "esfuzz": "~0.3.1",
        "estraverse": "~1.5.1",
        "mocha": "~2.3.4"
    },
    "directories": {},
    "dist": {
        "shasum": "d286190b6eefc6fd65eb0ecac6551e0b0e8839a4",
        "tarball": "https://registry.npmjs.org/uglify-js/-/uglify-js-2.8.16.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "files": [
        "bin",
        "lib",
        "tools",
        "LICENSE"
    ],
    "gitHead": "491f16c766c92e20260b99696b6081f333ceaf0f",
    "homepage": "http://lisperator.net/uglifyjs",
    "keywords": [
        "uglify",
        "uglify-js",
        "minify",
        "minifier"
    ],
    "license": "BSD-2-Clause",
    "main": "tools/node.js",
    "maintainers": [
        {
            "name": "alexlamsl",
            "email": "alexlamsl@gmail.com"
        },
        {
            "name": "mishoo",
            "email": "mihai.bazon@gmail.com"
        },
        {
            "name": "rvanvelzen1",
            "email": "rvanvelzen1@gmail.com"
        }
    ],
    "name": "uglify-js",
    "optionalDependencies": {
        "uglify-to-browserify": "~1.0.0"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mishoo/UglifyJS2.git"
    },
    "scripts": {
        "test": "node test/run-tests.js"
    },
    "version": "2.8.16"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module uglify-js](#apidoc.module.uglify-js)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Accessor (props)](#apidoc.element.uglify-js.AST_Accessor)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Array (props)](#apidoc.element.uglify-js.AST_Array)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Assign (props)](#apidoc.element.uglify-js.AST_Assign)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Atom (props)](#apidoc.element.uglify-js.AST_Atom)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Binary (props)](#apidoc.element.uglify-js.AST_Binary)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Block (props)](#apidoc.element.uglify-js.AST_Block)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_BlockStatement (props)](#apidoc.element.uglify-js.AST_BlockStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Boolean (props)](#apidoc.element.uglify-js.AST_Boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Break (props)](#apidoc.element.uglify-js.AST_Break)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Call (props)](#apidoc.element.uglify-js.AST_Call)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Case (props)](#apidoc.element.uglify-js.AST_Case)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Catch (props)](#apidoc.element.uglify-js.AST_Catch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Conditional (props)](#apidoc.element.uglify-js.AST_Conditional)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Const (props)](#apidoc.element.uglify-js.AST_Const)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Constant (props)](#apidoc.element.uglify-js.AST_Constant)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Continue (props)](#apidoc.element.uglify-js.AST_Continue)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_DWLoop (props)](#apidoc.element.uglify-js.AST_DWLoop)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Debugger (props)](#apidoc.element.uglify-js.AST_Debugger)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Default (props)](#apidoc.element.uglify-js.AST_Default)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Definitions (props)](#apidoc.element.uglify-js.AST_Definitions)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Defun (props)](#apidoc.element.uglify-js.AST_Defun)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Directive (props)](#apidoc.element.uglify-js.AST_Directive)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Do (props)](#apidoc.element.uglify-js.AST_Do)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Dot (props)](#apidoc.element.uglify-js.AST_Dot)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_EmptyStatement (props)](#apidoc.element.uglify-js.AST_EmptyStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Exit (props)](#apidoc.element.uglify-js.AST_Exit)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_False (props)](#apidoc.element.uglify-js.AST_False)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Finally (props)](#apidoc.element.uglify-js.AST_Finally)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_For (props)](#apidoc.element.uglify-js.AST_For)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ForIn (props)](#apidoc.element.uglify-js.AST_ForIn)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Function (props)](#apidoc.element.uglify-js.AST_Function)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Hole (props)](#apidoc.element.uglify-js.AST_Hole)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_If (props)](#apidoc.element.uglify-js.AST_If)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Infinity (props)](#apidoc.element.uglify-js.AST_Infinity)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_IterationStatement (props)](#apidoc.element.uglify-js.AST_IterationStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Jump (props)](#apidoc.element.uglify-js.AST_Jump)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Label (props)](#apidoc.element.uglify-js.AST_Label)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabelRef (props)](#apidoc.element.uglify-js.AST_LabelRef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabeledStatement (props)](#apidoc.element.uglify-js.AST_LabeledStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Lambda (props)](#apidoc.element.uglify-js.AST_Lambda)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_LoopControl (props)](#apidoc.element.uglify-js.AST_LoopControl)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_NaN (props)](#apidoc.element.uglify-js.AST_NaN)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_New (props)](#apidoc.element.uglify-js.AST_New)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Node (props)](#apidoc.element.uglify-js.AST_Node)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Null (props)](#apidoc.element.uglify-js.AST_Null)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Number (props)](#apidoc.element.uglify-js.AST_Number)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Object (props)](#apidoc.element.uglify-js.AST_Object)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectGetter (props)](#apidoc.element.uglify-js.AST_ObjectGetter)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectProperty (props)](#apidoc.element.uglify-js.AST_ObjectProperty)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectSetter (props)](#apidoc.element.uglify-js.AST_ObjectSetter)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_PropAccess (props)](#apidoc.element.uglify-js.AST_PropAccess)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_RegExp (props)](#apidoc.element.uglify-js.AST_RegExp)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Return (props)](#apidoc.element.uglify-js.AST_Return)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Scope (props)](#apidoc.element.uglify-js.AST_Scope)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Seq (props)](#apidoc.element.uglify-js.AST_Seq)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SimpleStatement (props)](#apidoc.element.uglify-js.AST_SimpleStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Statement (props)](#apidoc.element.uglify-js.AST_Statement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_StatementWithBody (props)](#apidoc.element.uglify-js.AST_StatementWithBody)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_String (props)](#apidoc.element.uglify-js.AST_String)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Sub (props)](#apidoc.element.uglify-js.AST_Sub)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Switch (props)](#apidoc.element.uglify-js.AST_Switch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SwitchBranch (props)](#apidoc.element.uglify-js.AST_SwitchBranch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Symbol (props)](#apidoc.element.uglify-js.AST_Symbol)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolAccessor (props)](#apidoc.element.uglify-js.AST_SymbolAccessor)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolCatch (props)](#apidoc.element.uglify-js.AST_SymbolCatch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolConst (props)](#apidoc.element.uglify-js.AST_SymbolConst)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDefun (props)](#apidoc.element.uglify-js.AST_SymbolDefun)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolFunarg (props)](#apidoc.element.uglify-js.AST_SymbolFunarg)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolLambda (props)](#apidoc.element.uglify-js.AST_SymbolLambda)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolRef (props)](#apidoc.element.uglify-js.AST_SymbolRef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolVar (props)](#apidoc.element.uglify-js.AST_SymbolVar)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_This (props)](#apidoc.element.uglify-js.AST_This)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Throw (props)](#apidoc.element.uglify-js.AST_Throw)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Token (props)](#apidoc.element.uglify-js.AST_Token)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Toplevel (props)](#apidoc.element.uglify-js.AST_Toplevel)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_True (props)](#apidoc.element.uglify-js.AST_True)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Try (props)](#apidoc.element.uglify-js.AST_Try)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Unary (props)](#apidoc.element.uglify-js.AST_Unary)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPostfix (props)](#apidoc.element.uglify-js.AST_UnaryPostfix)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPrefix (props)](#apidoc.element.uglify-js.AST_UnaryPrefix)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Undefined (props)](#apidoc.element.uglify-js.AST_Undefined)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Var (props)](#apidoc.element.uglify-js.AST_Var)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_VarDef (props)](#apidoc.element.uglify-js.AST_VarDef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_While (props)](#apidoc.element.uglify-js.AST_While)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_With (props)](#apidoc.element.uglify-js.AST_With)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>Compressor (options, false_by_default)](#apidoc.element.uglify-js.Compressor)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>DefaultsError (msg, defs)](#apidoc.element.uglify-js.DefaultsError)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>Dictionary ()](#apidoc.element.uglify-js.Dictionary)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglify-js.JS_Parse_Error)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>MAP (a, f, backwards)](#apidoc.element.uglify-js.MAP)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>OutputStream (options)](#apidoc.element.uglify-js.OutputStream)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>SourceMap (options)](#apidoc.element.uglify-js.SourceMap)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglify-js.SymbolDef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>TreeTransformer (before, after)](#apidoc.element.uglify-js.TreeTransformer)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>TreeWalker (callback)](#apidoc.element.uglify-js.TreeWalker)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>base54 (num)](#apidoc.element.uglify-js.base54)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>defaults (args, defs, croak)](#apidoc.element.uglify-js.defaults)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>describe_ast ()](#apidoc.element.uglify-js.describe_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>is_identifier (name)](#apidoc.element.uglify-js.is_identifier)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>mangle_properties (ast, options)](#apidoc.element.uglify-js.mangle_properties)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>merge (obj, ext)](#apidoc.element.uglify-js.merge)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>minify (files, options)](#apidoc.element.uglify-js.minify)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>parse ($TEXT, options)](#apidoc.element.uglify-js.parse)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>push_uniq (array, el)](#apidoc.element.uglify-js.push_uniq)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>readDefaultReservedFile (reserved)](#apidoc.element.uglify-js.readDefaultReservedFile)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>readNameCache (filename, key)](#apidoc.element.uglify-js.readNameCache)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>readReservedFile (filename, reserved)](#apidoc.element.uglify-js.readReservedFile)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>simple_glob (glob)](#apidoc.element.uglify-js.simple_glob)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>string_template (text, props)](#apidoc.element.uglify-js.string_template)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>tokenizer ($TEXT, filename, html5_comments, shebang)](#apidoc.element.uglify-js.tokenizer)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>writeNameCache (filename, key, cache)](#apidoc.element.uglify-js.writeNameCache)
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Accessor.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Array.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Assign.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Atom.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Atom.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Binary.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Binary.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Block.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Block.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_BlockStatement.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Boolean.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Boolean.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Break.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Call.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Call.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Case.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Catch.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Conditional.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Const.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Constant.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Constant.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Continue.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_DWLoop.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_DWLoop.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Debugger.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Default.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Definitions.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Definitions.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Defun.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Directive.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Do.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Dot.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_EmptyStatement.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Exit.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Exit.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_False.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Finally.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_For.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_ForIn.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Function.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Hole.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_If.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Infinity.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_IterationStatement.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_IterationStatement.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Jump.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Jump.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Label.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_LabelRef.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_LabeledStatement.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Lambda.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Lambda.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_LoopControl.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_LoopControl.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_NaN.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_New.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Node.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Node.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Null.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Number.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Object.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectGetter.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectKeyVal.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectProperty.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectProperty.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectSetter.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_PropAccess.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_PropAccess.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_RegExp.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Return.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Scope.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Scope.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Seq.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SimpleStatement.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Statement.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Statement.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_StatementWithBody.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_StatementWithBody.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_String.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Sub.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Switch.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SwitchBranch.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SwitchBranch.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Symbol.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Symbol.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolAccessor.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolCatch.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolConst.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDeclaration.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDeclaration.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDefun.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolFunarg.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolLambda.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolRef.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolVar.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolVar.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_This.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Throw.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Token.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Toplevel.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_True.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Try.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Unary.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Unary.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPostfix.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPrefix.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Undefined.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_Var.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_VarDef.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_While.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>AST_With.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>Compressor.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>DefaultsError.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>Dictionary.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>FILES
1.  object <span class="apidocSignatureSpan">uglify-js.</span>JS_Parse_Error.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>SymbolDef.prototype
1.  object <span class="apidocSignatureSpan">uglify-js.</span>TreeWalker.prototype

#### [module uglify-js.AST_Accessor](#apidoc.module.uglify-js.AST_Accessor)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Accessor (props)](#apidoc.element.uglify-js.AST_Accessor.AST_Accessor)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>BASE (props)](#apidoc.element.uglify-js.AST_Accessor.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Accessor.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>documentation

#### [module uglify-js.AST_Accessor.prototype](#apidoc.module.uglify-js.AST_Accessor.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Accessor.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Accessor.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Accessor.prototype.</span>TYPE

#### [module uglify-js.AST_Array](#apidoc.module.uglify-js.AST_Array)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Array (props)](#apidoc.element.uglify-js.AST_Array.AST_Array)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>BASE (props)](#apidoc.element.uglify-js.AST_Array.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Array.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>documentation

#### [module uglify-js.AST_Array.prototype](#apidoc.module.uglify-js.AST_Array.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Array.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Array.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_Array.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Array.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Array.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Array.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Array.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Array.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Array.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>TYPE

#### [module uglify-js.AST_Assign](#apidoc.module.uglify-js.AST_Assign)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Assign (props)](#apidoc.element.uglify-js.AST_Assign.AST_Assign)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>BASE (props)](#apidoc.element.uglify-js.AST_Assign.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Assign.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>documentation

#### [module uglify-js.AST_Assign.prototype](#apidoc.module.uglify-js.AST_Assign.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Assign.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Assign.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Assign.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Assign.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Assign.prototype.is_number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Assign.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Assign.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Assign.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Assign.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>TYPE

#### [module uglify-js.AST_Atom](#apidoc.module.uglify-js.AST_Atom)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Atom (props)](#apidoc.element.uglify-js.AST_Atom.AST_Atom)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>BASE (props)](#apidoc.element.uglify-js.AST_Atom.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Atom.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>documentation

#### [module uglify-js.AST_Atom.SUBCLASSES](#apidoc.module.uglify-js.AST_Atom.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.5)

#### [module uglify-js.AST_Atom.prototype](#apidoc.module.uglify-js.AST_Atom.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Atom.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Atom.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Atom.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Atom.prototype.</span>TYPE

#### [module uglify-js.AST_Binary](#apidoc.module.uglify-js.AST_Binary)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Binary (props)](#apidoc.element.uglify-js.AST_Binary.AST_Binary)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>BASE (props)](#apidoc.element.uglify-js.AST_Binary.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Binary.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>documentation

#### [module uglify-js.AST_Binary.SUBCLASSES](#apidoc.module.uglify-js.AST_Binary.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Binary.SUBCLASSES.0)

#### [module uglify-js.AST_Binary.prototype](#apidoc.module.uglify-js.AST_Binary.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Binary.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Binary.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>_eval (c)](#apidoc.element.uglify-js.AST_Binary.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Binary.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Binary.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Binary.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.is_number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.lift_sequences)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Binary.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Binary.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Binary.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Binary.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>TYPE

#### [module uglify-js.AST_Block](#apidoc.module.uglify-js.AST_Block)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Block (props)](#apidoc.element.uglify-js.AST_Block.AST_Block)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>BASE (props)](#apidoc.element.uglify-js.AST_Block.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Block.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>documentation

#### [module uglify-js.AST_Block.SUBCLASSES](#apidoc.module.uglify-js.AST_Block.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.5)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>6 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.6)

#### [module uglify-js.AST_Block.prototype](#apidoc.module.uglify-js.AST_Block.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Block.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Block.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Block.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Block.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Block.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Block.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>TYPE

#### [module uglify-js.AST_BlockStatement](#apidoc.module.uglify-js.AST_BlockStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_BlockStatement (props)](#apidoc.element.uglify-js.AST_BlockStatement.AST_BlockStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_BlockStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_BlockStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>documentation

#### [module uglify-js.AST_BlockStatement.prototype](#apidoc.module.uglify-js.AST_BlockStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_BlockStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_BlockStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_BlockStatement.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_BlockStatement.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_BlockStatement.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_BlockStatement.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>TYPE

#### [module uglify-js.AST_Boolean](#apidoc.module.uglify-js.AST_Boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Boolean (props)](#apidoc.element.uglify-js.AST_Boolean.AST_Boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>BASE (props)](#apidoc.element.uglify-js.AST_Boolean.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Boolean.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>documentation

#### [module uglify-js.AST_Boolean.SUBCLASSES](#apidoc.module.uglify-js.AST_Boolean.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Boolean.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Boolean.SUBCLASSES.1)

#### [module uglify-js.AST_Boolean.prototype](#apidoc.module.uglify-js.AST_Boolean.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Boolean.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Boolean.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Boolean.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Boolean.prototype.</span>TYPE

#### [module uglify-js.AST_Break](#apidoc.module.uglify-js.AST_Break)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Break (props)](#apidoc.element.uglify-js.AST_Break.AST_Break)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>BASE (props)](#apidoc.element.uglify-js.AST_Break.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Break.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>documentation

#### [module uglify-js.AST_Break.prototype](#apidoc.module.uglify-js.AST_Break.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Break.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Break.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Break.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Break.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Break.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Break.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Break.prototype.</span>TYPE

#### [module uglify-js.AST_Call](#apidoc.module.uglify-js.AST_Call)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Call (props)](#apidoc.element.uglify-js.AST_Call.AST_Call)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>BASE (props)](#apidoc.element.uglify-js.AST_Call.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Call.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>documentation

#### [module uglify-js.AST_Call.SUBCLASSES](#apidoc.module.uglify-js.AST_Call.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Call.SUBCLASSES.0)

#### [module uglify-js.AST_Call.prototype](#apidoc.module.uglify-js.AST_Call.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Call.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Call.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Call.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Call.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>has_pure_annotation (compressor)](#apidoc.element.uglify-js.AST_Call.prototype.has_pure_annotation)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Call.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Call.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Call.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Call.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Call.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>TYPE

#### [module uglify-js.AST_Case](#apidoc.module.uglify-js.AST_Case)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Case (props)](#apidoc.element.uglify-js.AST_Case.AST_Case)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>BASE (props)](#apidoc.element.uglify-js.AST_Case.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Case.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>documentation

#### [module uglify-js.AST_Case.prototype](#apidoc.module.uglify-js.AST_Case.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Case.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Case.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Case.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Case.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Case.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>TYPE

#### [module uglify-js.AST_Catch](#apidoc.module.uglify-js.AST_Catch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Catch (props)](#apidoc.element.uglify-js.AST_Catch.AST_Catch)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>BASE (props)](#apidoc.element.uglify-js.AST_Catch.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Catch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>documentation

#### [module uglify-js.AST_Catch.prototype](#apidoc.module.uglify-js.AST_Catch.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Catch.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Catch.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Catch.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Catch.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Catch.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Catch.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>TYPE

#### [module uglify-js.AST_Conditional](#apidoc.module.uglify-js.AST_Conditional)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Conditional (props)](#apidoc.element.uglify-js.AST_Conditional.AST_Conditional)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>BASE (props)](#apidoc.element.uglify-js.AST_Conditional.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Conditional.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>documentation

#### [module uglify-js.AST_Conditional.prototype](#apidoc.module.uglify-js.AST_Conditional.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Conditional.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Conditional.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Conditional.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>drop_side_effect_free (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Conditional.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.is_number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Conditional.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Conditional.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Conditional.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Conditional.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>TYPE

#### [module uglify-js.AST_Const](#apidoc.module.uglify-js.AST_Const)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Const (props)](#apidoc.element.uglify-js.AST_Const.AST_Const)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>BASE (props)](#apidoc.element.uglify-js.AST_Const.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Const.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>documentation

#### [module uglify-js.AST_Const.prototype](#apidoc.module.uglify-js.AST_Const.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Const.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Const.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Const.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Const.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Const.prototype.</span>TYPE

#### [module uglify-js.AST_Constant](#apidoc.module.uglify-js.AST_Constant)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Constant (props)](#apidoc.element.uglify-js.AST_Constant.AST_Constant)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>BASE (props)](#apidoc.element.uglify-js.AST_Constant.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Constant.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>documentation

#### [module uglify-js.AST_Constant.SUBCLASSES](#apidoc.module.uglify-js.AST_Constant.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.3)

#### [module uglify-js.AST_Constant.prototype](#apidoc.module.uglify-js.AST_Constant.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Constant.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Constant.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Constant.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Constant.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Constant.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>getValue ()](#apidoc.element.uglify-js.AST_Constant.prototype.getValue)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Constant.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Constant.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>TYPE

#### [module uglify-js.AST_Continue](#apidoc.module.uglify-js.AST_Continue)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Continue (props)](#apidoc.element.uglify-js.AST_Continue.AST_Continue)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>BASE (props)](#apidoc.element.uglify-js.AST_Continue.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Continue.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>documentation

#### [module uglify-js.AST_Continue.prototype](#apidoc.module.uglify-js.AST_Continue.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Continue.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Continue.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Continue.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Continue.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Continue.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Continue.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Continue.prototype.</span>TYPE

#### [module uglify-js.AST_DWLoop](#apidoc.module.uglify-js.AST_DWLoop)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_DWLoop (props)](#apidoc.element.uglify-js.AST_DWLoop.AST_DWLoop)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>BASE (props)](#apidoc.element.uglify-js.AST_DWLoop.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_DWLoop.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>documentation

#### [module uglify-js.AST_DWLoop.SUBCLASSES](#apidoc.module.uglify-js.AST_DWLoop.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_DWLoop.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_DWLoop.SUBCLASSES.1)

#### [module uglify-js.AST_DWLoop.prototype](#apidoc.module.uglify-js.AST_DWLoop.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_DWLoop.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_DWLoop.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_DWLoop.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.prototype.</span>TYPE

#### [module uglify-js.AST_Debugger](#apidoc.module.uglify-js.AST_Debugger)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Debugger (props)](#apidoc.element.uglify-js.AST_Debugger.AST_Debugger)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>BASE (props)](#apidoc.element.uglify-js.AST_Debugger.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Debugger.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>documentation

#### [module uglify-js.AST_Debugger.prototype](#apidoc.module.uglify-js.AST_Debugger.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Debugger.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Debugger.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Debugger.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Debugger.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Debugger.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>TYPE

#### [module uglify-js.AST_Default](#apidoc.module.uglify-js.AST_Default)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Default (props)](#apidoc.element.uglify-js.AST_Default.AST_Default)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>BASE (props)](#apidoc.element.uglify-js.AST_Default.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Default.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>documentation

#### [module uglify-js.AST_Default.prototype](#apidoc.module.uglify-js.AST_Default.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Default.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Default.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Default.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Default.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Default.prototype.</span>TYPE

#### [module uglify-js.AST_Definitions](#apidoc.module.uglify-js.AST_Definitions)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Definitions (props)](#apidoc.element.uglify-js.AST_Definitions.AST_Definitions)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>BASE (props)](#apidoc.element.uglify-js.AST_Definitions.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Definitions.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>documentation

#### [module uglify-js.AST_Definitions.SUBCLASSES](#apidoc.module.uglify-js.AST_Definitions.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Definitions.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Definitions.SUBCLASSES.1)

#### [module uglify-js.AST_Definitions.prototype](#apidoc.module.uglify-js.AST_Definitions.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Definitions.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>_do_print (output, kind)](#apidoc.element.uglify-js.AST_Definitions.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Definitions.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Definitions.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Definitions.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>remove_initializers ()](#apidoc.element.uglify-js.AST_Definitions.prototype.remove_initializers)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>to_assignments (compressor)](#apidoc.element.uglify-js.AST_Definitions.prototype.to_assignments)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Definitions.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Definitions.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>TYPE

#### [module uglify-js.AST_Defun](#apidoc.module.uglify-js.AST_Defun)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Defun (props)](#apidoc.element.uglify-js.AST_Defun.AST_Defun)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>BASE (props)](#apidoc.element.uglify-js.AST_Defun.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Defun.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>documentation

#### [module uglify-js.AST_Defun.prototype](#apidoc.module.uglify-js.AST_Defun.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Defun.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Defun.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Defun.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Defun.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Defun.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Defun.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Defun.prototype.</span>TYPE

#### [module uglify-js.AST_Directive](#apidoc.module.uglify-js.AST_Directive)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Directive (props)](#apidoc.element.uglify-js.AST_Directive.AST_Directive)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>BASE (props)](#apidoc.element.uglify-js.AST_Directive.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Directive.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>documentation

#### [module uglify-js.AST_Directive.prototype](#apidoc.module.uglify-js.AST_Directive.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Directive.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Directive.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Directive.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Directive.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Directive.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>TYPE

#### [module uglify-js.AST_Do](#apidoc.module.uglify-js.AST_Do)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Do (props)](#apidoc.element.uglify-js.AST_Do.AST_Do)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>BASE (props)](#apidoc.element.uglify-js.AST_Do.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Do.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>documentation

#### [module uglify-js.AST_Do.prototype](#apidoc.module.uglify-js.AST_Do.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Do.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Do.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Do.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Do.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>TYPE

#### [module uglify-js.AST_Dot](#apidoc.module.uglify-js.AST_Dot)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Dot (props)](#apidoc.element.uglify-js.AST_Dot.AST_Dot)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>BASE (props)](#apidoc.element.uglify-js.AST_Dot.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Dot.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>documentation

#### [module uglify-js.AST_Dot.prototype](#apidoc.module.uglify-js.AST_Dot.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Dot.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Dot.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>_find_defs (compressor, suffix)](#apidoc.element.uglify-js.AST_Dot.prototype._find_defs)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Dot.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Dot.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Dot.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Dot.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Dot.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>TYPE

#### [module uglify-js.AST_EmptyStatement](#apidoc.module.uglify-js.AST_EmptyStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_EmptyStatement (props)](#apidoc.element.uglify-js.AST_EmptyStatement.AST_EmptyStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_EmptyStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_EmptyStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>documentation

#### [module uglify-js.AST_EmptyStatement.prototype](#apidoc.module.uglify-js.AST_EmptyStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_EmptyStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_EmptyStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_EmptyStatement.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_EmptyStatement.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_EmptyStatement.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>TYPE

#### [module uglify-js.AST_Exit](#apidoc.module.uglify-js.AST_Exit)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Exit (props)](#apidoc.element.uglify-js.AST_Exit.AST_Exit)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>BASE (props)](#apidoc.element.uglify-js.AST_Exit.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Exit.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>documentation

#### [module uglify-js.AST_Exit.SUBCLASSES](#apidoc.module.uglify-js.AST_Exit.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Exit.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Exit.SUBCLASSES.1)

#### [module uglify-js.AST_Exit.prototype](#apidoc.module.uglify-js.AST_Exit.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Exit.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>_do_print (output, kind)](#apidoc.element.uglify-js.AST_Exit.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Exit.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Exit.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>TYPE

#### [module uglify-js.AST_False](#apidoc.module.uglify-js.AST_False)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_False (props)](#apidoc.element.uglify-js.AST_False.AST_False)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_False.</span>BASE (props)](#apidoc.element.uglify-js.AST_False.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_False.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_False.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_False.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_False.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_False.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_False.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_False.</span>documentation

#### [module uglify-js.AST_False.prototype](#apidoc.module.uglify-js.AST_False.prototype)
1.  boolean <span class="apidocSignatureSpan">uglify-js.AST_False.prototype.</span>value
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_False.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_False.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_False.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_False.prototype.is_boolean)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_False.prototype.</span>TYPE

#### [module uglify-js.AST_Finally](#apidoc.module.uglify-js.AST_Finally)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Finally (props)](#apidoc.element.uglify-js.AST_Finally.AST_Finally)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>BASE (props)](#apidoc.element.uglify-js.AST_Finally.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Finally.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>documentation

#### [module uglify-js.AST_Finally.prototype](#apidoc.module.uglify-js.AST_Finally.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Finally.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Finally.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Finally.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Finally.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Finally.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Finally.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Finally.prototype.</span>TYPE

#### [module uglify-js.AST_For](#apidoc.module.uglify-js.AST_For)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_For (props)](#apidoc.element.uglify-js.AST_For.AST_For)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.</span>BASE (props)](#apidoc.element.uglify-js.AST_For.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_For.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_For.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_For.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_For.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_For.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_For.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_For.</span>documentation

#### [module uglify-js.AST_For.prototype](#apidoc.module.uglify-js.AST_For.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_For.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_For.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_For.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_For.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_For.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_For.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>TYPE

#### [module uglify-js.AST_ForIn](#apidoc.module.uglify-js.AST_ForIn)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ForIn (props)](#apidoc.element.uglify-js.AST_ForIn.AST_ForIn)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>BASE (props)](#apidoc.element.uglify-js.AST_ForIn.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ForIn.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>documentation

#### [module uglify-js.AST_ForIn.prototype](#apidoc.module.uglify-js.AST_ForIn.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ForIn.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ForIn.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_ForIn.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_ForIn.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_ForIn.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>TYPE

#### [module uglify-js.AST_Function](#apidoc.module.uglify-js.AST_Function)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Function (props)](#apidoc.element.uglify-js.AST_Function.AST_Function)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>BASE (props)](#apidoc.element.uglify-js.AST_Function.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Function.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>documentation

#### [module uglify-js.AST_Function.prototype](#apidoc.module.uglify-js.AST_Function.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Function.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Function.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Function.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Function.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Function.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>next_mangled (options, def)](#apidoc.element.uglify-js.AST_Function.prototype.next_mangled)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Function.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>TYPE

#### [module uglify-js.AST_Hole](#apidoc.module.uglify-js.AST_Hole)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Hole (props)](#apidoc.element.uglify-js.AST_Hole.AST_Hole)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>BASE (props)](#apidoc.element.uglify-js.AST_Hole.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Hole.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>documentation

#### [module uglify-js.AST_Hole.prototype](#apidoc.module.uglify-js.AST_Hole.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Hole.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Hole.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Hole.prototype.</span>_codegen ()](#apidoc.element.uglify-js.AST_Hole.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Hole.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Hole.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Hole.prototype.</span>TYPE

#### [module uglify-js.AST_If](#apidoc.module.uglify-js.AST_If)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_If (props)](#apidoc.element.uglify-js.AST_If.AST_If)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.</span>BASE (props)](#apidoc.element.uglify-js.AST_If.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_If.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_If.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_If.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_If.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_If.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_If.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_If.</span>documentation

#### [module uglify-js.AST_If.prototype](#apidoc.module.uglify-js.AST_If.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_If.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_If.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_If.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_If.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_If.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_If.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_If.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>TYPE

#### [module uglify-js.AST_Infinity](#apidoc.module.uglify-js.AST_Infinity)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Infinity (props)](#apidoc.element.uglify-js.AST_Infinity.AST_Infinity)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>BASE (props)](#apidoc.element.uglify-js.AST_Infinity.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Infinity.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>documentation

#### [module uglify-js.AST_Infinity.prototype](#apidoc.module.uglify-js.AST_Infinity.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Infinity.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Infinity.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Infinity.prototype.optimize)
1.  number <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>value
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>TYPE

#### [module uglify-js.AST_IterationStatement](#apidoc.module.uglify-js.AST_IterationStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_IterationStatement (props)](#apidoc.element.uglify-js.AST_IterationStatement.AST_IterationStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_IterationStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_IterationStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>documentation

#### [module uglify-js.AST_IterationStatement.SUBCLASSES](#apidoc.module.uglify-js.AST_IterationStatement.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.2)

#### [module uglify-js.AST_IterationStatement.prototype](#apidoc.module.uglify-js.AST_IterationStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_IterationStatement.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.prototype.</span>TYPE

#### [module uglify-js.AST_Jump](#apidoc.module.uglify-js.AST_Jump)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Jump (props)](#apidoc.element.uglify-js.AST_Jump.AST_Jump)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>BASE (props)](#apidoc.element.uglify-js.AST_Jump.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Jump.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>documentation

#### [module uglify-js.AST_Jump.SUBCLASSES](#apidoc.module.uglify-js.AST_Jump.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Jump.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Jump.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Jump.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Jump.SUBCLASSES.1)

#### [module uglify-js.AST_Jump.prototype](#apidoc.module.uglify-js.AST_Jump.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Jump.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Jump.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Jump.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_Jump.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Jump.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Jump.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Jump.prototype.</span>TYPE

#### [module uglify-js.AST_Label](#apidoc.module.uglify-js.AST_Label)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Label (props)](#apidoc.element.uglify-js.AST_Label.AST_Label)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>BASE (props)](#apidoc.element.uglify-js.AST_Label.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Label.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>documentation

#### [module uglify-js.AST_Label.prototype](#apidoc.module.uglify-js.AST_Label.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Label.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>initialize ()](#apidoc.element.uglify-js.AST_Label.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>undeclared ()](#apidoc.element.uglify-js.AST_Label.prototype.undeclared)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>unmangleable ()](#apidoc.element.uglify-js.AST_Label.prototype.unmangleable)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>TYPE

#### [module uglify-js.AST_LabelRef](#apidoc.module.uglify-js.AST_LabelRef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabelRef (props)](#apidoc.element.uglify-js.AST_LabelRef.AST_LabelRef)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>BASE (props)](#apidoc.element.uglify-js.AST_LabelRef.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_LabelRef.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>documentation

#### [module uglify-js.AST_LabelRef.prototype](#apidoc.module.uglify-js.AST_LabelRef.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_LabelRef.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.prototype.</span>undeclared ()](#apidoc.element.uglify-js.AST_LabelRef.prototype.undeclared)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.prototype.</span>TYPE

#### [module uglify-js.AST_LabeledStatement](#apidoc.module.uglify-js.AST_LabeledStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabeledStatement (props)](#apidoc.element.uglify-js.AST_LabeledStatement.AST_LabeledStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_LabeledStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_LabeledStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>documentation

#### [module uglify-js.AST_LabeledStatement.prototype](#apidoc.module.uglify-js.AST_LabeledStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>clone (deep)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.clone)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>TYPE

#### [module uglify-js.AST_Lambda](#apidoc.module.uglify-js.AST_Lambda)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Lambda (props)](#apidoc.element.uglify-js.AST_Lambda.AST_Lambda)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>BASE (props)](#apidoc.element.uglify-js.AST_Lambda.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Lambda.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>documentation

#### [module uglify-js.AST_Lambda.SUBCLASSES](#apidoc.module.uglify-js.AST_Lambda.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.2)

#### [module uglify-js.AST_Lambda.prototype](#apidoc.module.uglify-js.AST_Lambda.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Lambda.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Lambda.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_do_print (output, nokeyword)](#apidoc.element.uglify-js.AST_Lambda.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Lambda.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Lambda.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Lambda.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>init_scope_vars ()](#apidoc.element.uglify-js.AST_Lambda.prototype.init_scope_vars)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Lambda.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Lambda.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>TYPE

#### [module uglify-js.AST_LoopControl](#apidoc.module.uglify-js.AST_LoopControl)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_LoopControl (props)](#apidoc.element.uglify-js.AST_LoopControl.AST_LoopControl)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>BASE (props)](#apidoc.element.uglify-js.AST_LoopControl.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_LoopControl.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>documentation

#### [module uglify-js.AST_LoopControl.SUBCLASSES](#apidoc.module.uglify-js.AST_LoopControl.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_LoopControl.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_LoopControl.SUBCLASSES.1)

#### [module uglify-js.AST_LoopControl.prototype](#apidoc.module.uglify-js.AST_LoopControl.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_LoopControl.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>_do_print (output, kind)](#apidoc.element.uglify-js.AST_LoopControl.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_LoopControl.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_LoopControl.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>TYPE

#### [module uglify-js.AST_NaN](#apidoc.module.uglify-js.AST_NaN)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_NaN (props)](#apidoc.element.uglify-js.AST_NaN.AST_NaN)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>BASE (props)](#apidoc.element.uglify-js.AST_NaN.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_NaN.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>documentation

#### [module uglify-js.AST_NaN.prototype](#apidoc.module.uglify-js.AST_NaN.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_NaN.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_NaN.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_NaN.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_NaN.prototype._codegen)
1.  number <span class="apidocSignatureSpan">uglify-js.AST_NaN.prototype.</span>value
1.  string <span class="apidocSignatureSpan">uglify-js.AST_NaN.prototype.</span>TYPE

#### [module uglify-js.AST_New](#apidoc.module.uglify-js.AST_New)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_New (props)](#apidoc.element.uglify-js.AST_New.AST_New)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.</span>BASE (props)](#apidoc.element.uglify-js.AST_New.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_New.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_New.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_New.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_New.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_New.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_New.</span>documentation

#### [module uglify-js.AST_New.prototype](#apidoc.module.uglify-js.AST_New.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_New.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_New.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_New.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_New.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_New.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_New.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>TYPE

#### [module uglify-js.AST_Node](#apidoc.module.uglify-js.AST_Node)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Node (props)](#apidoc.element.uglify-js.AST_Node.AST_Node)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Node.DEFMETHOD)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>from_mozilla_ast (node)](#apidoc.element.uglify-js.AST_Node.from_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>warn (txt, props)](#apidoc.element.uglify-js.AST_Node.warn)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>warn_function (txt)](#apidoc.element.uglify-js.AST_Node.warn_function)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>documentation

#### [module uglify-js.AST_Node.SUBCLASSES](#apidoc.module.uglify-js.AST_Node.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>10 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.10)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>11 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.11)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>12 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.12)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.5)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>6 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.6)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>7 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.7)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>8 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.8)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>9 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.9)

#### [module uglify-js.AST_Node.prototype](#apidoc.module.uglify-js.AST_Node.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Node.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_clone (deep)](#apidoc.element.uglify-js.AST_Node.prototype._clone)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Node.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_find_defs ()](#apidoc.element.uglify-js.AST_Node.prototype._find_defs)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Node.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>add_comments (output)](#apidoc.element.uglify-js.AST_Node.prototype.add_comments)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Node.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>clone (deep)](#apidoc.element.uglify-js.AST_Node.prototype.clone)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>constant_value (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.constant_value)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Node.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>equivalent_to (node)](#apidoc.element.uglify-js.AST_Node.prototype.equivalent_to)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>evaluate (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Node.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Node.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_constant ()](#apidoc.element.uglify-js.AST_Node.prototype.is_constant)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_number ()](#apidoc.element.uglify-js.AST_Node.prototype.is_number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_string ()](#apidoc.element.uglify-js.AST_Node.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>needs_parens ()](#apidoc.element.uglify-js.AST_Node.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Node.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>print (stream, force_parens)](#apidoc.element.uglify-js.AST_Node.prototype.print)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>print_to_string (options)](#apidoc.element.uglify-js.AST_Node.prototype.print_to_string)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>process_expression (insert)](#apidoc.element.uglify-js.AST_Node.prototype.process_expression)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>reset_opt_flags (compressor, rescan)](#apidoc.element.uglify-js.AST_Node.prototype.reset_opt_flags)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>resolve_defines (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.resolve_defines)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Node.prototype.transform)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>walk (visitor)](#apidoc.element.uglify-js.AST_Node.prototype.walk)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>TYPE

#### [module uglify-js.AST_Null](#apidoc.module.uglify-js.AST_Null)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Null (props)](#apidoc.element.uglify-js.AST_Null.AST_Null)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>BASE (props)](#apidoc.element.uglify-js.AST_Null.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Null.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>documentation

#### [module uglify-js.AST_Null.prototype](#apidoc.module.uglify-js.AST_Null.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Null.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Null.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Null.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Null.prototype.to_mozilla_ast)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Null.prototype.</span>value
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Null.prototype.</span>TYPE

#### [module uglify-js.AST_Number](#apidoc.module.uglify-js.AST_Number)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Number (props)](#apidoc.element.uglify-js.AST_Number.AST_Number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>BASE (props)](#apidoc.element.uglify-js.AST_Number.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Number.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>documentation

#### [module uglify-js.AST_Number.prototype](#apidoc.module.uglify-js.AST_Number.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Number.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Number.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>is_number ()](#apidoc.element.uglify-js.AST_Number.prototype.is_number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Number.prototype.needs_parens)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>TYPE

#### [module uglify-js.AST_Object](#apidoc.module.uglify-js.AST_Object)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Object (props)](#apidoc.element.uglify-js.AST_Object.AST_Object)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>BASE (props)](#apidoc.element.uglify-js.AST_Object.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Object.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>documentation

#### [module uglify-js.AST_Object.prototype](#apidoc.module.uglify-js.AST_Object.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Object.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Object.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_Object.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Object.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Object.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Object.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Object.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Object.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Object.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Object.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>TYPE

#### [module uglify-js.AST_ObjectGetter](#apidoc.module.uglify-js.AST_ObjectGetter)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectGetter (props)](#apidoc.element.uglify-js.AST_ObjectGetter.AST_ObjectGetter)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectGetter.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectGetter.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>documentation

#### [module uglify-js.AST_ObjectGetter.prototype](#apidoc.module.uglify-js.AST_ObjectGetter.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectGetter.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ObjectGetter.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_ObjectGetter.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.prototype.</span>TYPE

#### [module uglify-js.AST_ObjectKeyVal](#apidoc.module.uglify-js.AST_ObjectKeyVal)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal.AST_ObjectKeyVal)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectKeyVal.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>documentation

#### [module uglify-js.AST_ObjectKeyVal.prototype](#apidoc.module.uglify-js.AST_ObjectKeyVal.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ObjectKeyVal.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.prototype.</span>TYPE

#### [module uglify-js.AST_ObjectProperty](#apidoc.module.uglify-js.AST_ObjectProperty)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectProperty (props)](#apidoc.element.uglify-js.AST_ObjectProperty.AST_ObjectProperty)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectProperty.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectProperty.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>documentation

#### [module uglify-js.AST_ObjectProperty.SUBCLASSES](#apidoc.module.uglify-js.AST_ObjectProperty.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.2)

#### [module uglify-js.AST_ObjectProperty.prototype](#apidoc.module.uglify-js.AST_ObjectProperty.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>TYPE

#### [module uglify-js.AST_ObjectSetter](#apidoc.module.uglify-js.AST_ObjectSetter)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectSetter (props)](#apidoc.element.uglify-js.AST_ObjectSetter.AST_ObjectSetter)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectSetter.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectSetter.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>documentation

#### [module uglify-js.AST_ObjectSetter.prototype](#apidoc.module.uglify-js.AST_ObjectSetter.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectSetter.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ObjectSetter.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_ObjectSetter.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.prototype.</span>TYPE

#### [module uglify-js.AST_PropAccess](#apidoc.module.uglify-js.AST_PropAccess)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_PropAccess (props)](#apidoc.element.uglify-js.AST_PropAccess.AST_PropAccess)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>BASE (props)](#apidoc.element.uglify-js.AST_PropAccess.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_PropAccess.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>documentation

#### [module uglify-js.AST_PropAccess.SUBCLASSES](#apidoc.module.uglify-js.AST_PropAccess.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_PropAccess.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_PropAccess.SUBCLASSES.1)

#### [module uglify-js.AST_PropAccess.prototype](#apidoc.module.uglify-js.AST_PropAccess.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_PropAccess.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_PropAccess.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_PropAccess.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_PropAccess.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_PropAccess.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>TYPE

#### [module uglify-js.AST_RegExp](#apidoc.module.uglify-js.AST_RegExp)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_RegExp (props)](#apidoc.element.uglify-js.AST_RegExp.AST_RegExp)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>BASE (props)](#apidoc.element.uglify-js.AST_RegExp.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_RegExp.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>documentation

#### [module uglify-js.AST_RegExp.prototype](#apidoc.module.uglify-js.AST_RegExp.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_RegExp.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_RegExp.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_RegExp.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_RegExp.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>TYPE

#### [module uglify-js.AST_Return](#apidoc.module.uglify-js.AST_Return)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Return (props)](#apidoc.element.uglify-js.AST_Return.AST_Return)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>BASE (props)](#apidoc.element.uglify-js.AST_Return.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Return.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>documentation

#### [module uglify-js.AST_Return.prototype](#apidoc.module.uglify-js.AST_Return.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Return.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Return.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Return.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Return.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>TYPE

#### [module uglify-js.AST_Scope](#apidoc.module.uglify-js.AST_Scope)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Scope (props)](#apidoc.element.uglify-js.AST_Scope.AST_Scope)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>BASE (props)](#apidoc.element.uglify-js.AST_Scope.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Scope.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>documentation

#### [module uglify-js.AST_Scope.SUBCLASSES](#apidoc.module.uglify-js.AST_Scope.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Scope.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Scope.SUBCLASSES.1)

#### [module uglify-js.AST_Scope.prototype](#apidoc.module.uglify-js.AST_Scope.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Scope.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>def_function (symbol)](#apidoc.element.uglify-js.AST_Scope.prototype.def_function)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>def_variable (symbol)](#apidoc.element.uglify-js.AST_Scope.prototype.def_variable)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>drop_unused (compressor)](#apidoc.element.uglify-js.AST_Scope.prototype.drop_unused)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>find_variable (name)](#apidoc.element.uglify-js.AST_Scope.prototype.find_variable)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>hoist_declarations (compressor)](#apidoc.element.uglify-js.AST_Scope.prototype.hoist_declarations)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>init_scope_vars ()](#apidoc.element.uglify-js.AST_Scope.prototype.init_scope_vars)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>next_mangled (options)](#apidoc.element.uglify-js.AST_Scope.prototype.next_mangled)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>TYPE

#### [module uglify-js.AST_Seq](#apidoc.module.uglify-js.AST_Seq)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Seq (props)](#apidoc.element.uglify-js.AST_Seq.AST_Seq)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>BASE (props)](#apidoc.element.uglify-js.AST_Seq.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Seq.DEFMETHOD)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>cons (x, y)](#apidoc.element.uglify-js.AST_Seq.cons)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>from_array (array)](#apidoc.element.uglify-js.AST_Seq.from_array)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>documentation

#### [module uglify-js.AST_Seq.prototype](#apidoc.module.uglify-js.AST_Seq.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Seq.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Seq.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>_do_print (output)](#apidoc.element.uglify-js.AST_Seq.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Seq.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>add (node)](#apidoc.element.uglify-js.AST_Seq.prototype.add)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>drop_side_effect_free (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Seq.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.is_number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>len ()](#apidoc.element.uglify-js.AST_Seq.prototype.len)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Seq.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Seq.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>to_array ()](#apidoc.element.uglify-js.AST_Seq.prototype.to_array)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Seq.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Seq.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>TYPE

#### [module uglify-js.AST_SimpleStatement](#apidoc.module.uglify-js.AST_SimpleStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SimpleStatement (props)](#apidoc.element.uglify-js.AST_SimpleStatement.AST_SimpleStatement)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_SimpleStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SimpleStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>documentation

#### [module uglify-js.AST_SimpleStatement.prototype](#apidoc.module.uglify-js.AST_SimpleStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>TYPE

#### [module uglify-js.AST_Statement](#apidoc.module.uglify-js.AST_Statement)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Statement (props)](#apidoc.element.uglify-js.AST_Statement.AST_Statement)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>BASE (props)](#apidoc.element.uglify-js.AST_Statement.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Statement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>documentation

#### [module uglify-js.AST_Statement.SUBCLASSES](#apidoc.module.uglify-js.AST_Statement.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.5)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>6 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.6)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>7 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.7)

#### [module uglify-js.AST_Statement.prototype](#apidoc.module.uglify-js.AST_Statement.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Statement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Statement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Statement.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_Statement.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Statement.prototype.negate)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>TYPE

#### [module uglify-js.AST_StatementWithBody](#apidoc.module.uglify-js.AST_StatementWithBody)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_StatementWithBody (props)](#apidoc.element.uglify-js.AST_StatementWithBody.AST_StatementWithBody)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>BASE (props)](#apidoc.element.uglify-js.AST_StatementWithBody.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_StatementWithBody.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>documentation

#### [module uglify-js.AST_StatementWithBody.SUBCLASSES](#apidoc.module.uglify-js.AST_StatementWithBody.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.3)

#### [module uglify-js.AST_StatementWithBody.prototype](#apidoc.module.uglify-js.AST_StatementWithBody.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>_do_print_body (output)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype._do_print_body)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>TYPE

#### [module uglify-js.AST_String](#apidoc.module.uglify-js.AST_String)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_String (props)](#apidoc.element.uglify-js.AST_String.AST_String)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_String.</span>BASE (props)](#apidoc.element.uglify-js.AST_String.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_String.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_String.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_String.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_String.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_String.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_String.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_String.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_String.</span>documentation

#### [module uglify-js.AST_String.prototype](#apidoc.module.uglify-js.AST_String.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_String.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_String.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_String.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_String.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_String.prototype.</span>is_string ()](#apidoc.element.uglify-js.AST_String.prototype.is_string)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_String.prototype.</span>TYPE

#### [module uglify-js.AST_Sub](#apidoc.module.uglify-js.AST_Sub)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Sub (props)](#apidoc.element.uglify-js.AST_Sub.AST_Sub)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>BASE (props)](#apidoc.element.uglify-js.AST_Sub.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Sub.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>documentation

#### [module uglify-js.AST_Sub.prototype](#apidoc.module.uglify-js.AST_Sub.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Sub.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Sub.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Sub.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Sub.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Sub.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Sub.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Sub.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>TYPE

#### [module uglify-js.AST_Switch](#apidoc.module.uglify-js.AST_Switch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Switch (props)](#apidoc.element.uglify-js.AST_Switch.AST_Switch)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>BASE (props)](#apidoc.element.uglify-js.AST_Switch.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Switch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>documentation

#### [module uglify-js.AST_Switch.prototype](#apidoc.module.uglify-js.AST_Switch.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Switch.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Switch.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Switch.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Switch.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Switch.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Switch.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Switch.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>TYPE

#### [module uglify-js.AST_SwitchBranch](#apidoc.module.uglify-js.AST_SwitchBranch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SwitchBranch (props)](#apidoc.element.uglify-js.AST_SwitchBranch.AST_SwitchBranch)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>BASE (props)](#apidoc.element.uglify-js.AST_SwitchBranch.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SwitchBranch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>documentation

#### [module uglify-js.AST_SwitchBranch.SUBCLASSES](#apidoc.module.uglify-js.AST_SwitchBranch.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_SwitchBranch.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_SwitchBranch.SUBCLASSES.1)

#### [module uglify-js.AST_SwitchBranch.prototype](#apidoc.module.uglify-js.AST_SwitchBranch.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>_do_print_body (output)](#apidoc.element.uglify-js.AST_SwitchBranch.prototype._do_print_body)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>TYPE

#### [module uglify-js.AST_Symbol](#apidoc.module.uglify-js.AST_Symbol)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Symbol (props)](#apidoc.element.uglify-js.AST_Symbol.AST_Symbol)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>BASE (props)](#apidoc.element.uglify-js.AST_Symbol.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Symbol.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>documentation

#### [module uglify-js.AST_Symbol.SUBCLASSES](#apidoc.module.uglify-js.AST_Symbol.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.5)

#### [module uglify-js.AST_Symbol.prototype](#apidoc.module.uglify-js.AST_Symbol.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Symbol.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Symbol.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Symbol.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>definition ()](#apidoc.element.uglify-js.AST_Symbol.prototype.definition)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>global ()](#apidoc.element.uglify-js.AST_Symbol.prototype.global)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Symbol.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>undeclared ()](#apidoc.element.uglify-js.AST_Symbol.prototype.undeclared)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>unmangleable (options)](#apidoc.element.uglify-js.AST_Symbol.prototype.unmangleable)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>unreferenced ()](#apidoc.element.uglify-js.AST_Symbol.prototype.unreferenced)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolAccessor](#apidoc.module.uglify-js.AST_SymbolAccessor)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolAccessor (props)](#apidoc.element.uglify-js.AST_SymbolAccessor.AST_SymbolAccessor)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolAccessor.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolAccessor.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>documentation

#### [module uglify-js.AST_SymbolAccessor.prototype](#apidoc.module.uglify-js.AST_SymbolAccessor.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolAccessor.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.prototype.</span>unmangleable ()](#apidoc.element.uglify-js.AST_SymbolAccessor.prototype.unmangleable)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolCatch](#apidoc.module.uglify-js.AST_SymbolCatch)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolCatch (props)](#apidoc.element.uglify-js.AST_SymbolCatch.AST_SymbolCatch)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolCatch.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolCatch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>documentation

#### [module uglify-js.AST_SymbolCatch.prototype](#apidoc.module.uglify-js.AST_SymbolCatch.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolCatch.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolConst](#apidoc.module.uglify-js.AST_SymbolConst)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolConst (props)](#apidoc.element.uglify-js.AST_SymbolConst.AST_SymbolConst)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolConst.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolConst.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>documentation

#### [module uglify-js.AST_SymbolConst.prototype](#apidoc.module.uglify-js.AST_SymbolConst.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolConst.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolDeclaration](#apidoc.module.uglify-js.AST_SymbolDeclaration)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.AST_SymbolDeclaration)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolDeclaration.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>documentation

#### [module uglify-js.AST_SymbolDeclaration.SUBCLASSES](#apidoc.module.uglify-js.AST_SymbolDeclaration.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.4)

#### [module uglify-js.AST_SymbolDeclaration.prototype](#apidoc.module.uglify-js.AST_SymbolDeclaration.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolDefun](#apidoc.module.uglify-js.AST_SymbolDefun)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDefun (props)](#apidoc.element.uglify-js.AST_SymbolDefun.AST_SymbolDefun)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolDefun.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolDefun.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>documentation

#### [module uglify-js.AST_SymbolDefun.prototype](#apidoc.module.uglify-js.AST_SymbolDefun.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolDefun.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolFunarg](#apidoc.module.uglify-js.AST_SymbolFunarg)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolFunarg (props)](#apidoc.element.uglify-js.AST_SymbolFunarg.AST_SymbolFunarg)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolFunarg.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolFunarg.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>documentation

#### [module uglify-js.AST_SymbolFunarg.prototype](#apidoc.module.uglify-js.AST_SymbolFunarg.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolFunarg.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolLambda](#apidoc.module.uglify-js.AST_SymbolLambda)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolLambda (props)](#apidoc.element.uglify-js.AST_SymbolLambda.AST_SymbolLambda)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolLambda.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolLambda.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>documentation

#### [module uglify-js.AST_SymbolLambda.prototype](#apidoc.module.uglify-js.AST_SymbolLambda.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolLambda.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolRef](#apidoc.module.uglify-js.AST_SymbolRef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolRef (props)](#apidoc.element.uglify-js.AST_SymbolRef.AST_SymbolRef)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolRef.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolRef.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>documentation

#### [module uglify-js.AST_SymbolRef.prototype](#apidoc.module.uglify-js.AST_SymbolRef.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_SymbolRef.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>_find_defs (compressor, suffix)](#apidoc.element.uglify-js.AST_SymbolRef.prototype._find_defs)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_SymbolRef.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>reference (options)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.reference)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>TYPE

#### [module uglify-js.AST_SymbolVar](#apidoc.module.uglify-js.AST_SymbolVar)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolVar (props)](#apidoc.element.uglify-js.AST_SymbolVar.AST_SymbolVar)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolVar.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolVar.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>documentation

#### [module uglify-js.AST_SymbolVar.SUBCLASSES](#apidoc.module.uglify-js.AST_SymbolVar.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_SymbolVar.SUBCLASSES.0)

#### [module uglify-js.AST_SymbolVar.prototype](#apidoc.module.uglify-js.AST_SymbolVar.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolVar.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.prototype.</span>TYPE

#### [module uglify-js.AST_This](#apidoc.module.uglify-js.AST_This)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_This (props)](#apidoc.element.uglify-js.AST_This.AST_This)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_This.</span>BASE (props)](#apidoc.element.uglify-js.AST_This.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_This.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_This.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_This.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_This.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_This.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_This.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_This.</span>documentation

#### [module uglify-js.AST_This.prototype](#apidoc.module.uglify-js.AST_This.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_This.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_This.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_This.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_This.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_This.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>TYPE

#### [module uglify-js.AST_Throw](#apidoc.module.uglify-js.AST_Throw)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Throw (props)](#apidoc.element.uglify-js.AST_Throw.AST_Throw)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>BASE (props)](#apidoc.element.uglify-js.AST_Throw.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Throw.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>documentation

#### [module uglify-js.AST_Throw.prototype](#apidoc.module.uglify-js.AST_Throw.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Throw.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Throw.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Throw.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Throw.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Throw.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Throw.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Throw.prototype.</span>TYPE

#### [module uglify-js.AST_Token](#apidoc.module.uglify-js.AST_Token)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Token (props)](#apidoc.element.uglify-js.AST_Token.AST_Token)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Token.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Token.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Token.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Token.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Token.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Token.</span>TYPE

#### [module uglify-js.AST_Token.prototype](#apidoc.module.uglify-js.AST_Token.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Token.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Token.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Token.prototype.</span>TYPE

#### [module uglify-js.AST_Toplevel](#apidoc.module.uglify-js.AST_Toplevel)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Toplevel (props)](#apidoc.element.uglify-js.AST_Toplevel.AST_Toplevel)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>BASE (props)](#apidoc.element.uglify-js.AST_Toplevel.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Toplevel.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>documentation

#### [module uglify-js.AST_Toplevel.prototype](#apidoc.module.uglify-js.AST_Toplevel.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Toplevel.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Toplevel.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>_default_mangler_options (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype._default_mangler_options)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Toplevel.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>compute_char_frequency (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.compute_char_frequency)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>def_global (node)](#apidoc.element.uglify-js.AST_Toplevel.prototype.def_global)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>figure_out_scope (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.figure_out_scope)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>mangle_names (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.mangle_names)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>scope_warnings (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.scope_warnings)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Toplevel.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>wrap_commonjs (name, export_all)](#apidoc.element.uglify-js.AST_Toplevel.prototype.wrap_commonjs)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>wrap_enclose (arg_parameter_pairs)](#apidoc.element.uglify-js.AST_Toplevel.prototype.wrap_enclose)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>TYPE

#### [module uglify-js.AST_True](#apidoc.module.uglify-js.AST_True)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_True (props)](#apidoc.element.uglify-js.AST_True.AST_True)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_True.</span>BASE (props)](#apidoc.element.uglify-js.AST_True.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_True.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_True.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_True.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_True.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_True.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_True.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_True.</span>documentation

#### [module uglify-js.AST_True.prototype](#apidoc.module.uglify-js.AST_True.prototype)
1.  boolean <span class="apidocSignatureSpan">uglify-js.AST_True.prototype.</span>value
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_True.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_True.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_True.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_True.prototype.is_boolean)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_True.prototype.</span>TYPE

#### [module uglify-js.AST_Try](#apidoc.module.uglify-js.AST_Try)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Try (props)](#apidoc.element.uglify-js.AST_Try.AST_Try)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>BASE (props)](#apidoc.element.uglify-js.AST_Try.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Try.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>documentation

#### [module uglify-js.AST_Try.prototype](#apidoc.module.uglify-js.AST_Try.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Try.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Try.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Try.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Try.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Try.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Try.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Try.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>TYPE

#### [module uglify-js.AST_Unary](#apidoc.module.uglify-js.AST_Unary)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Unary (props)](#apidoc.element.uglify-js.AST_Unary.AST_Unary)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>BASE (props)](#apidoc.element.uglify-js.AST_Unary.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Unary.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>documentation

#### [module uglify-js.AST_Unary.SUBCLASSES](#apidoc.module.uglify-js.AST_Unary.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Unary.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Unary.SUBCLASSES.1)

#### [module uglify-js.AST_Unary.prototype](#apidoc.module.uglify-js.AST_Unary.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Unary.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Unary.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Unary.prototype.drop_side_effect_free)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Unary.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>is_number ()](#apidoc.element.uglify-js.AST_Unary.prototype.is_number)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglify-js.AST_Unary.prototype.lift_sequences)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Unary.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Unary.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Unary.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>TYPE

#### [module uglify-js.AST_UnaryPostfix](#apidoc.module.uglify-js.AST_UnaryPostfix)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPostfix (props)](#apidoc.element.uglify-js.AST_UnaryPostfix.AST_UnaryPostfix)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>BASE (props)](#apidoc.element.uglify-js.AST_UnaryPostfix.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_UnaryPostfix.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>documentation

#### [module uglify-js.AST_UnaryPostfix.prototype](#apidoc.module.uglify-js.AST_UnaryPostfix.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_UnaryPostfix.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_UnaryPostfix.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_UnaryPostfix.prototype.optimize)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.prototype.</span>TYPE

#### [module uglify-js.AST_UnaryPrefix](#apidoc.module.uglify-js.AST_UnaryPrefix)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPrefix (props)](#apidoc.element.uglify-js.AST_UnaryPrefix.AST_UnaryPrefix)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>BASE (props)](#apidoc.element.uglify-js.AST_UnaryPrefix.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_UnaryPrefix.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>documentation

#### [module uglify-js.AST_UnaryPrefix.prototype](#apidoc.module.uglify-js.AST_UnaryPrefix.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>is_string ()](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.optimize)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>TYPE

#### [module uglify-js.AST_Undefined](#apidoc.module.uglify-js.AST_Undefined)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Undefined (props)](#apidoc.element.uglify-js.AST_Undefined.AST_Undefined)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>BASE (props)](#apidoc.element.uglify-js.AST_Undefined.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Undefined.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>documentation

#### [module uglify-js.AST_Undefined.prototype](#apidoc.module.uglify-js.AST_Undefined.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Undefined.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Undefined.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Undefined.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Undefined.prototype.optimize)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>TYPE

#### [module uglify-js.AST_Var](#apidoc.module.uglify-js.AST_Var)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_Var (props)](#apidoc.element.uglify-js.AST_Var.AST_Var)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>BASE (props)](#apidoc.element.uglify-js.AST_Var.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Var.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>documentation

#### [module uglify-js.AST_Var.prototype](#apidoc.module.uglify-js.AST_Var.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Var.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Var.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_Var.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Var.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_Var.prototype.</span>TYPE

#### [module uglify-js.AST_VarDef](#apidoc.module.uglify-js.AST_VarDef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_VarDef (props)](#apidoc.element.uglify-js.AST_VarDef.AST_VarDef)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>BASE (props)](#apidoc.element.uglify-js.AST_VarDef.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_VarDef.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>documentation

#### [module uglify-js.AST_VarDef.prototype](#apidoc.module.uglify-js.AST_VarDef.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_VarDef.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_VarDef.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_VarDef.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_VarDef.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_VarDef.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_VarDef.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>TYPE

#### [module uglify-js.AST_While](#apidoc.module.uglify-js.AST_While)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_While (props)](#apidoc.element.uglify-js.AST_While.AST_While)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_While.</span>BASE (props)](#apidoc.element.uglify-js.AST_While.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_While.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_While.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_While.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_While.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_While.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglify-js.AST_While.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_While.</span>documentation

#### [module uglify-js.AST_While.prototype](#apidoc.module.uglify-js.AST_While.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_While.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_While.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_While.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_While.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>TYPE

#### [module uglify-js.AST_With](#apidoc.module.uglify-js.AST_With)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>AST_With (props)](#apidoc.element.uglify-js.AST_With.AST_With)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_With.</span>BASE (props)](#apidoc.element.uglify-js.AST_With.BASE)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_With.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_With.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglify-js.AST_With.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_With.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglify-js.AST_With.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglify-js.AST_With.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglify-js.AST_With.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglify-js.AST_With.</span>documentation

#### [module uglify-js.AST_With.prototype](#apidoc.module.uglify-js.AST_With.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_With.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_With.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_With.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_With.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_With.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>TYPE

#### [module uglify-js.Compressor](#apidoc.module.uglify-js.Compressor)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>Compressor (options, false_by_default)](#apidoc.element.uglify-js.Compressor.Compressor)

#### [module uglify-js.Compressor.prototype](#apidoc.module.uglify-js.Compressor.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>before (node, descend, in_list)](#apidoc.element.uglify-js.Compressor.prototype.before)
1.  [function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>clear_warnings ()](#apidoc.element.uglify-js.Compressor.prototype.clear_warnings)
1.  [function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>compress (node)](#apidoc.element.uglify-js.Compressor.prototype.compress)
1.  [function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>info ()](#apidoc.element.uglify-js.Compressor.prototype.info)
1.  [function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>option (key)](#apidoc.element.uglify-js.Compressor.prototype.option)
1.  [function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>warn (text, props)](#apidoc.element.uglify-js.Compressor.prototype.warn)
1.  object <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>directives
1.  object <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>stack

#### [module uglify-js.DefaultsError](#apidoc.module.uglify-js.DefaultsError)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>DefaultsError (msg, defs)](#apidoc.element.uglify-js.DefaultsError.DefaultsError)
1.  [function <span class="apidocSignatureSpan">uglify-js.DefaultsError.</span>croak (msg, defs)](#apidoc.element.uglify-js.DefaultsError.croak)

#### [module uglify-js.DefaultsError.prototype](#apidoc.module.uglify-js.DefaultsError.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.DefaultsError.prototype.</span>constructor (msg, defs)](#apidoc.element.uglify-js.DefaultsError.prototype.constructor)
1.  string <span class="apidocSignatureSpan">uglify-js.DefaultsError.prototype.</span>name

#### [module uglify-js.Dictionary](#apidoc.module.uglify-js.Dictionary)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>Dictionary ()](#apidoc.element.uglify-js.Dictionary.Dictionary)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.</span>fromObject (obj)](#apidoc.element.uglify-js.Dictionary.fromObject)

#### [module uglify-js.Dictionary.prototype](#apidoc.module.uglify-js.Dictionary.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>add (key, val)](#apidoc.element.uglify-js.Dictionary.prototype.add)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>del (key)](#apidoc.element.uglify-js.Dictionary.prototype.del)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>each (f)](#apidoc.element.uglify-js.Dictionary.prototype.each)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>get (key)](#apidoc.element.uglify-js.Dictionary.prototype.get)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>has (key)](#apidoc.element.uglify-js.Dictionary.prototype.has)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>map (f)](#apidoc.element.uglify-js.Dictionary.prototype.map)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>set (key, val)](#apidoc.element.uglify-js.Dictionary.prototype.set)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>size ()](#apidoc.element.uglify-js.Dictionary.prototype.size)
1.  [function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>toObject ()](#apidoc.element.uglify-js.Dictionary.prototype.toObject)

#### [module uglify-js.JS_Parse_Error](#apidoc.module.uglify-js.JS_Parse_Error)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglify-js.JS_Parse_Error.JS_Parse_Error)

#### [module uglify-js.JS_Parse_Error.prototype](#apidoc.module.uglify-js.JS_Parse_Error.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.JS_Parse_Error.prototype.</span>constructor (message, filename, line, col, pos)](#apidoc.element.uglify-js.JS_Parse_Error.prototype.constructor)
1.  string <span class="apidocSignatureSpan">uglify-js.JS_Parse_Error.prototype.</span>name

#### [module uglify-js.MAP](#apidoc.module.uglify-js.MAP)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>MAP (a, f, backwards)](#apidoc.element.uglify-js.MAP.MAP)
1.  [function <span class="apidocSignatureSpan">uglify-js.MAP.</span>at_top (val)](#apidoc.element.uglify-js.MAP.at_top)
1.  [function <span class="apidocSignatureSpan">uglify-js.MAP.</span>last (val)](#apidoc.element.uglify-js.MAP.last)
1.  [function <span class="apidocSignatureSpan">uglify-js.MAP.</span>splice (val)](#apidoc.element.uglify-js.MAP.splice)
1.  object <span class="apidocSignatureSpan">uglify-js.MAP.</span>skip

#### [module uglify-js.SymbolDef](#apidoc.module.uglify-js.SymbolDef)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglify-js.SymbolDef.SymbolDef)
1.  number <span class="apidocSignatureSpan">uglify-js.SymbolDef.</span>next_id

#### [module uglify-js.SymbolDef.prototype](#apidoc.module.uglify-js.SymbolDef.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.SymbolDef.prototype.</span>mangle (options)](#apidoc.element.uglify-js.SymbolDef.prototype.mangle)
1.  [function <span class="apidocSignatureSpan">uglify-js.SymbolDef.prototype.</span>unmangleable (options)](#apidoc.element.uglify-js.SymbolDef.prototype.unmangleable)

#### [module uglify-js.TreeWalker](#apidoc.module.uglify-js.TreeWalker)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>TreeWalker (callback)](#apidoc.element.uglify-js.TreeWalker.TreeWalker)

#### [module uglify-js.TreeWalker.prototype](#apidoc.module.uglify-js.TreeWalker.prototype)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>_visit (node, descend)](#apidoc.element.uglify-js.TreeWalker.prototype._visit)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>find_parent (type)](#apidoc.element.uglify-js.TreeWalker.prototype.find_parent)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>has_directive (type)](#apidoc.element.uglify-js.TreeWalker.prototype.has_directive)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>in_boolean_context ()](#apidoc.element.uglify-js.TreeWalker.prototype.in_boolean_context)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>loopcontrol_target (label)](#apidoc.element.uglify-js.TreeWalker.prototype.loopcontrol_target)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>parent (n)](#apidoc.element.uglify-js.TreeWalker.prototype.parent)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>pop (node)](#apidoc.element.uglify-js.TreeWalker.prototype.pop)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>push (node)](#apidoc.element.uglify-js.TreeWalker.prototype.push)
1.  [function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>self ()](#apidoc.element.uglify-js.TreeWalker.prototype.self)

#### [module uglify-js.base54](#apidoc.module.uglify-js.base54)
1.  [function <span class="apidocSignatureSpan">uglify-js.</span>base54 (num)](#apidoc.element.uglify-js.base54.base54)
1.  [function <span class="apidocSignatureSpan">uglify-js.base54.</span>consider (str)](#apidoc.element.uglify-js.base54.consider)
1.  [function <span class="apidocSignatureSpan">uglify-js.base54.</span>freq ()](#apidoc.element.uglify-js.base54.freq)
1.  [function <span class="apidocSignatureSpan">uglify-js.base54.</span>get ()](#apidoc.element.uglify-js.base54.get)
1.  [function <span class="apidocSignatureSpan">uglify-js.base54.</span>reset ()](#apidoc.element.uglify-js.base54.reset)
1.  [function <span class="apidocSignatureSpan">uglify-js.base54.</span>sort ()](#apidoc.element.uglify-js.base54.sort)



# <a name="apidoc.module.uglify-js"></a>[module uglify-js](#apidoc.module.uglify-js)

#### <a name="apidoc.element.uglify-js.AST_Accessor"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Accessor (props)](#apidoc.element.uglify-js.AST_Accessor)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Array (props)](#apidoc.element.uglify-js.AST_Array)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Assign (props)](#apidoc.element.uglify-js.AST_Assign)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Atom (props)](#apidoc.element.uglify-js.AST_Atom)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Binary (props)](#apidoc.element.uglify-js.AST_Binary)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Block (props)](#apidoc.element.uglify-js.AST_Block)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_BlockStatement (props)](#apidoc.element.uglify-js.AST_BlockStatement)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Boolean (props)](#apidoc.element.uglify-js.AST_Boolean)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Break"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Break (props)](#apidoc.element.uglify-js.AST_Break)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Call (props)](#apidoc.element.uglify-js.AST_Call)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Case"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Case (props)](#apidoc.element.uglify-js.AST_Case)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Catch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Catch (props)](#apidoc.element.uglify-js.AST_Catch)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Conditional (props)](#apidoc.element.uglify-js.AST_Conditional)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Const"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Const (props)](#apidoc.element.uglify-js.AST_Const)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Constant (props)](#apidoc.element.uglify-js.AST_Constant)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Continue"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Continue (props)](#apidoc.element.uglify-js.AST_Continue)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_DWLoop"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_DWLoop (props)](#apidoc.element.uglify-js.AST_DWLoop)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Debugger"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Debugger (props)](#apidoc.element.uglify-js.AST_Debugger)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Default"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Default (props)](#apidoc.element.uglify-js.AST_Default)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Definitions (props)](#apidoc.element.uglify-js.AST_Definitions)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Defun"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Defun (props)](#apidoc.element.uglify-js.AST_Defun)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Directive"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Directive (props)](#apidoc.element.uglify-js.AST_Directive)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Do"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Do (props)](#apidoc.element.uglify-js.AST_Do)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Dot (props)](#apidoc.element.uglify-js.AST_Dot)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_EmptyStatement (props)](#apidoc.element.uglify-js.AST_EmptyStatement)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Exit"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Exit (props)](#apidoc.element.uglify-js.AST_Exit)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_False"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_False (props)](#apidoc.element.uglify-js.AST_False)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Finally"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Finally (props)](#apidoc.element.uglify-js.AST_Finally)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_For"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_For (props)](#apidoc.element.uglify-js.AST_For)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ForIn"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ForIn (props)](#apidoc.element.uglify-js.AST_ForIn)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Function (props)](#apidoc.element.uglify-js.AST_Function)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Hole"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Hole (props)](#apidoc.element.uglify-js.AST_Hole)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_If (props)](#apidoc.element.uglify-js.AST_If)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Infinity"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Infinity (props)](#apidoc.element.uglify-js.AST_Infinity)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_IterationStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_IterationStatement (props)](#apidoc.element.uglify-js.AST_IterationStatement)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Jump"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Jump (props)](#apidoc.element.uglify-js.AST_Jump)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Label"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Label (props)](#apidoc.element.uglify-js.AST_Label)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabelRef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabelRef (props)](#apidoc.element.uglify-js.AST_LabelRef)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabeledStatement (props)](#apidoc.element.uglify-js.AST_LabeledStatement)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Lambda (props)](#apidoc.element.uglify-js.AST_Lambda)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LoopControl"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_LoopControl (props)](#apidoc.element.uglify-js.AST_LoopControl)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_NaN"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_NaN (props)](#apidoc.element.uglify-js.AST_NaN)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_New (props)](#apidoc.element.uglify-js.AST_New)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Node (props)](#apidoc.element.uglify-js.AST_Node)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Null"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Null (props)](#apidoc.element.uglify-js.AST_Null)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Number"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Number (props)](#apidoc.element.uglify-js.AST_Number)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.literal = props.literal;this.value =
props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Object (props)](#apidoc.element.uglify-js.AST_Object)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectGetter"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectGetter (props)](#apidoc.element.uglify-js.AST_ObjectGetter)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectKeyVal"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectProperty (props)](#apidoc.element.uglify-js.AST_ObjectProperty)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectSetter"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectSetter (props)](#apidoc.element.uglify-js.AST_ObjectSetter)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_PropAccess (props)](#apidoc.element.uglify-js.AST_PropAccess)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_RegExp"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_RegExp (props)](#apidoc.element.uglify-js.AST_RegExp)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Return"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Return (props)](#apidoc.element.uglify-js.AST_Return)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Scope (props)](#apidoc.element.uglify-js.AST_Scope)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Seq (props)](#apidoc.element.uglify-js.AST_Seq)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SimpleStatement (props)](#apidoc.element.uglify-js.AST_SimpleStatement)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Statement (props)](#apidoc.element.uglify-js.AST_Statement)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_StatementWithBody (props)](#apidoc.element.uglify-js.AST_StatementWithBody)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_String"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_String (props)](#apidoc.element.uglify-js.AST_String)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Sub (props)](#apidoc.element.uglify-js.AST_Sub)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Switch (props)](#apidoc.element.uglify-js.AST_Switch)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SwitchBranch (props)](#apidoc.element.uglify-js.AST_SwitchBranch)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Symbol (props)](#apidoc.element.uglify-js.AST_Symbol)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolAccessor"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolAccessor (props)](#apidoc.element.uglify-js.AST_SymbolAccessor)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolCatch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolCatch (props)](#apidoc.element.uglify-js.AST_SymbolCatch)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolConst"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolConst (props)](#apidoc.element.uglify-js.AST_SymbolConst)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDefun"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDefun (props)](#apidoc.element.uglify-js.AST_SymbolDefun)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolFunarg"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolFunarg (props)](#apidoc.element.uglify-js.AST_SymbolFunarg)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolLambda"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolLambda (props)](#apidoc.element.uglify-js.AST_SymbolLambda)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolRef (props)](#apidoc.element.uglify-js.AST_SymbolRef)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolVar"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolVar (props)](#apidoc.element.uglify-js.AST_SymbolVar)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_This"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_This (props)](#apidoc.element.uglify-js.AST_This)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Throw"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Throw (props)](#apidoc.element.uglify-js.AST_Throw)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Token"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Token (props)](#apidoc.element.uglify-js.AST_Token)
- description and source-code
```javascript
function AST_Token(props){ if (props) { this.raw = props.raw;this.file = props.file;this.comments_before = props.comments_before
;this.nlb = props.nlb;this.endpos = props.endpos;this.endcol = props.endcol;this.endline = props.endline;this.pos = props.pos;this
.col = props.col;this.line = props.line;this.value = props.value;this.type = props.type;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Toplevel (props)](#apidoc.element.uglify-js.AST_Toplevel)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_True"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_True (props)](#apidoc.element.uglify-js.AST_True)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Try (props)](#apidoc.element.uglify-js.AST_Try)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Unary (props)](#apidoc.element.uglify-js.AST_Unary)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPostfix"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPostfix (props)](#apidoc.element.uglify-js.AST_UnaryPostfix)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPrefix (props)](#apidoc.element.uglify-js.AST_UnaryPrefix)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Undefined"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Undefined (props)](#apidoc.element.uglify-js.AST_Undefined)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Var"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Var (props)](#apidoc.element.uglify-js.AST_Var)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_VarDef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_VarDef (props)](#apidoc.element.uglify-js.AST_VarDef)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_While"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_While (props)](#apidoc.element.uglify-js.AST_While)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_With"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_With (props)](#apidoc.element.uglify-js.AST_With)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Compressor"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>Compressor (options, false_by_default)](#apidoc.element.uglify-js.Compressor)
- description and source-code
```javascript
function Compressor(options, false_by_default) {
    if (!(this instanceof Compressor))
        return new Compressor(options, false_by_default);
    TreeTransformer.call(this, this.before, this.after);
    this.options = defaults(options, {
        sequences     : !false_by_default,
        properties    : !false_by_default,
        dead_code     : !false_by_default,
        drop_debugger : !false_by_default,
        unsafe        : false,
        unsafe_comps  : false,
        unsafe_math   : false,
        unsafe_proto  : false,
        conditionals  : !false_by_default,
        comparisons   : !false_by_default,
        evaluate      : !false_by_default,
        booleans      : !false_by_default,
        loops         : !false_by_default,
        unused        : !false_by_default,
        toplevel      : !!(options && options["top_retain"]),
        top_retain    : null,
        hoist_funs    : !false_by_default,
        keep_fargs    : true,
        keep_fnames   : false,
        hoist_vars    : false,
        if_return     : !false_by_default,
        join_vars     : !false_by_default,
        collapse_vars : !false_by_default,
        reduce_vars   : !false_by_default,
        cascade       : !false_by_default,
        side_effects  : !false_by_default,
        pure_getters  : false,
        pure_funcs    : null,
        negate_iife   : !false_by_default,
        screw_ie8     : true,
        drop_console  : false,
        angular       : false,
        expression    : false,
        warnings      : true,
        global_defs   : {},
        passes        : 1,
    }, true);
    var pure_funcs = this.options["pure_funcs"];
    if (typeof pure_funcs == "function") {
        this.pure_funcs = pure_funcs;
    } else {
        this.pure_funcs = pure_funcs ? function(node) {
            return pure_funcs.indexOf(node.expression.print_to_string()) < 0;
        } : return_true;
    }
    var top_retain = this.options["top_retain"];
    if (top_retain instanceof RegExp) {
        this.top_retain = function(def) {
            return top_retain.test(def.name);
        };
    } else if (typeof top_retain == "function") {
        this.top_retain = top_retain;
    } else if (top_retain) {
        if (typeof top_retain == "string") {
            top_retain = top_retain.split(/,/);
        }
        this.top_retain = function(def) {
            return top_retain.indexOf(def.name) >= 0;
        };
    }
    var sequences = this.options["sequences"];
    this.sequences_limit = sequences == 1 ? 200 : sequences | 0;
    this.warnings_produced = {};
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = UglifyJS.Compressor(options).compress(uAST);

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```

#### <a name="apidoc.element.uglify-js.DefaultsError"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>DefaultsError (msg, defs)](#apidoc.element.uglify-js.DefaultsError)
- description and source-code
```javascript
function DefaultsError(msg, defs) {
    this.message = msg;
    this.defs = defs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Dictionary"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>Dictionary ()](#apidoc.element.uglify-js.Dictionary)
- description and source-code
```javascript
function Dictionary() {
    this._values = Object.create(null);
    this._size = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.JS_Parse_Error"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglify-js.JS_Parse_Error)
- description and source-code
```javascript
function JS_Parse_Error(message, filename, line, col, pos) {
    this.message = message;
    this.filename = filename;
    this.line = line;
    this.col = col;
    this.pos = pos;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.MAP"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>MAP (a, f, backwards)](#apidoc.element.uglify-js.MAP)
- description and source-code
```javascript
function MAP(a, f, backwards) {
    var ret = [], top = [], i;
    function doit() {
        var val = f(a[i], i);
        var is_last = val instanceof Last;
        if (is_last) val = val.v;
        if (val instanceof AtTop) {
            val = val.v;
            if (val instanceof Splice) {
                top.push.apply(top, backwards ? val.v.slice().reverse() : val.v);
            } else {
                top.push(val);
            }
        }
        else if (val !== skip) {
            if (val instanceof Splice) {
                ret.push.apply(ret, backwards ? val.v.slice().reverse() : val.v);
            } else {
                ret.push(val);
            }
        }
        return is_last;
    };
    if (a instanceof Array) {
        if (backwards) {
            for (i = a.length; --i >= 0;) if (doit()) break;
            ret.reverse();
            top.reverse();
        } else {
            for (i = 0; i < a.length; ++i) if (doit()) break;
        }
    }
    else {
        for (i in a) if (HOP(a, i)) if (doit()) break;
    }
    return top.concat(ret);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.OutputStream"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>OutputStream (options)](#apidoc.element.uglify-js.OutputStream)
- description and source-code
```javascript
function OutputStream(options) {

    options = defaults(options, {
        indent_start     : 0,
        indent_level     : 4,
        quote_keys       : false,
        space_colon      : true,
        ascii_only       : false,
        unescape_regexps : false,
        inline_script    : false,
        width            : 80,
        max_line_len     : false,
        beautify         : false,
        source_map       : null,
        bracketize       : false,
        semicolons       : true,
        comments         : false,
        shebang          : true,
        preserve_line    : false,
        screw_ie8        : true,
        preamble         : null,
        quote_style      : 0,
        keep_quoted_props: false,
        wrap_iife        : false,
    }, true);

    // Convert comment option to RegExp if neccessary and set up comments filter
    var comment_filter = return_false; // Default case, throw all comments away
    if (options.comments) {
        var comments = options.comments;
        if (typeof options.comments === "string" && /^\/.*\/[a-zA-Z]*$/.test(options.comments)) {
            var regex_pos = options.comments.lastIndexOf("/");
            comments = new RegExp(
                options.comments.substr(1, regex_pos - 1),
                options.comments.substr(regex_pos + 1)
            );
        }
        if (comments instanceof RegExp) {
            comment_filter = function(comment) {
                return comment.type != "comment5" && comments.test(comment.value);
            };
        }
        else if (typeof comments === "function") {
            comment_filter = function(comment) {
                return comment.type != "comment5" && comments(this, comment);
            };
        }
        else if (comments === "some") {
            comment_filter = is_some_comments;
        } else { // NOTE includes "all" option
            comment_filter = return_true;
        }
    }

    var indentation = 0;
    var current_col = 0;
    var current_line = 1;
    var current_pos = 0;
    var OUTPUT = "";

    function to_ascii(str, identifier) {
        return str.replace(/[\u0000-\u001f\u007f-\uffff]/g, function(ch) {
            var code = ch.charCodeAt(0).toString(16);
            if (code.length <= 2 && !identifier) {
                while (code.length < 2) code = "0" + code;
                return "\\x" + code;
            } else {
                while (code.length < 4) code = "0" + code;
                return "\\u" + code;
            }
        });
    };

    function make_string(str, quote) {
        var dq = 0, sq = 0;
        str = str.replace(/[\\\b\f\n\r\v\t\x22\x27\u2028\u2029\0\ufeff]/g,
          function(s, i){
            switch (s) {
              case '"': ++dq; return '"';
              case "'": ++sq; return "'";
              case "\\": return "\\\\";
              case "\n": return "\\n";
              case "\r": return "\\r";
              case "\t": return "\\t";
              case "\b": return "\\b";
              case "\f": return "\\f";
              case "\x0B": return options.screw_ie8 ? "\\v" : "\\x0B";
              case "\u2028": return "\\u2028";
              case "\u2029": return "\\u2029";
              case "\ufeff": return "\\ufeff";
              case "\0":
                  return /[0-7]/.test(str.charAt(i+1)) ? "\\x00" : "\\0";
            }
            return s;
        });
        function quote_single() {
            return "'" + str.replace(/\x27/g, "\\'") + "'";
        }
        function quote_double() {
            return '"' + str.replace(/\x22/g, '\\"') + '"';
        }
        if (options.ascii_only) str = to_ascii(str);
        switch (options.quote_style) {
          case 1:
            return quote_single();
          case 2:
            return quote_double();
          case 3:
            return quote == "'" ? quote_single() : quote_double();
          default:
            return dq > sq ? quote_single() : quote_double();
        }
    };

    function encode_string(str, quote) {
        var ret = make_string(str, quote);
        if (options.inli ...
```
- example usage
```shell
...
'''

#### Generating output

AST nodes have a 'print' method that takes an output stream.  Essentially,
to generate code you do this:
'''javascript
var stream = UglifyJS.OutputStream(options);
compressed_ast.print(stream);
var code = stream.toString(); // this is your minified code
'''

or, for a shortcut you can do:
'''javascript
var code = compressed_ast.print_to_string(options);
...
```

#### <a name="apidoc.element.uglify-js.SourceMap"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>SourceMap (options)](#apidoc.element.uglify-js.SourceMap)
- description and source-code
```javascript
function SourceMap(options) {
    options = defaults(options, {
        file : null,
        root : null,
        orig : null,

        orig_line_diff : 0,
        dest_line_diff : 0,
    });
    var generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
    });
    var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);

    if (orig_map && Array.isArray(options.orig.sources)) {
        orig_map._sources.toArray().forEach(function(source) {
            var sourceContent = orig_map.sourceContentFor(source, true);
            if (sourceContent) {
                generator.setSourceContent(source, sourceContent);
            }
        });
    }

    function add(source, gen_line, gen_col, orig_line, orig_col, name) {
        if (orig_map) {
            var info = orig_map.originalPositionFor({
                line: orig_line,
                column: orig_col
            });
            if (info.source === null) {
                return;
            }
            source = info.source;
            orig_line = info.line;
            orig_col = info.column;
            name = info.name || name;
        }
        generator.addMapping({
            generated : { line: gen_line + options.dest_line_diff, column: gen_col },
            original  : { line: orig_line + options.orig_line_diff, column: orig_col },
            source    : source,
            name      : name
        });
    };
    return {
        add        : add,
        get        : function() { return generator },
        toString   : function() { return JSON.stringify(generator.toJSON()); }
    };
}
```
- example usage
```shell
...

You need to pass the 'source_map' argument when calling 'print'.  It needs
to be a 'SourceMap' object (which is a thin wrapper on top of the
[source-map][source-map] library).

Example:
'''javascript
var source_map = UglifyJS.SourceMap(source_map_options);
var stream = UglifyJS.OutputStream({
	...
	source_map: source_map
});
compressed_ast.print(stream);

var code = stream.toString();
...
```

#### <a name="apidoc.element.uglify-js.SymbolDef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglify-js.SymbolDef)
- description and source-code
```javascript
function SymbolDef(scope, index, orig) {
    this.name = orig.name;
    this.orig = [ orig ];
    this.scope = scope;
    this.references = [];
    this.global = false;
    this.mangled_name = null;
    this.undeclared = false;
    this.index = index;
    this.id = SymbolDef.next_id++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeTransformer"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>TreeTransformer (before, after)](#apidoc.element.uglify-js.TreeTransformer)
- description and source-code
```javascript
function TreeTransformer(before, after) {
    TreeWalker.call(this);
    this.before = before;
    this.after = after;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeWalker"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>TreeWalker (callback)](#apidoc.element.uglify-js.TreeWalker)
- description and source-code
```javascript
function TreeWalker(callback) {
    this.visit = callback;
    this.stack = [];
    this.directives = Object.create(null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.base54"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>base54 (num)](#apidoc.element.uglify-js.base54)
- description and source-code
```javascript
function base54(num) {
    var ret = "", base = 54;
    num++;
    do {
        num--;
        ret += String.fromCharCode(chars[num % base]);
        num = Math.floor(num / base);
        base = 64;
    } while (num > 0);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.defaults"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>defaults (args, defs, croak)](#apidoc.element.uglify-js.defaults)
- description and source-code
```javascript
function defaults(args, defs, croak) {
    if (args === true)
        args = {};
    var ret = args || {};
    if (croak) for (var i in ret) if (HOP(ret, i) && !HOP(defs, i))
        DefaultsError.croak("'" + i + "' is not a supported option", defs);
    for (var i in defs) if (HOP(defs, i)) {
        ret[i] = (args && HOP(args, i)) ? args[i] : defs[i];
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.describe_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>describe_ast ()](#apidoc.element.uglify-js.describe_ast)
- description and source-code
```javascript
describe_ast = function () {
    var out = UglifyJS.OutputStream({ beautify: true });
    function doitem(ctor) {
        out.print("AST_" + ctor.TYPE);
        var props = ctor.SELF_PROPS.filter(function(prop){
            return !/^\$/.test(prop);
        });
        if (props.length > 0) {
            out.space();
            out.with_parens(function(){
                props.forEach(function(prop, i){
                    if (i) out.space();
                    out.print(prop);
                });
            });
        }
        if (ctor.documentation) {
            out.space();
            out.print_string(ctor.documentation);
        }
        if (ctor.SUBCLASSES.length > 0) {
            out.space();
            out.with_block(function(){
                ctor.SUBCLASSES.forEach(function(ctor, i){
                    out.indent();
                    doitem(ctor);
                    out.newline();
                });
            });
        }
    };
    doitem(UglifyJS.AST_Node);
    return out + "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.is_identifier"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>is_identifier (name)](#apidoc.element.uglify-js.is_identifier)
- description and source-code
```javascript
function is_identifier(name) {
    return !RESERVED_WORDS(name) && /^[a-z_$][a-z0-9_$]*$/i.test(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.mangle_properties"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>mangle_properties (ast, options)](#apidoc.element.uglify-js.mangle_properties)
- description and source-code
```javascript
function mangle_properties(ast, options) {
    options = defaults(options, {
        reserved : null,
        cache : null,
        only_cache : false,
        regex : null,
        ignore_quoted : false,
        debug : false
    });

    var reserved = options.reserved;
    if (reserved == null)
        reserved = find_builtins();

    var cache = options.cache;
    if (cache == null) {
        cache = {
            cname: -1,
            props: new Dictionary()
        };
    }

    var regex = options.regex;
    var ignore_quoted = options.ignore_quoted;

    // note debug is either false (disabled), or a string of the debug suffix to use (enabled).
    // note debug may be enabled as an empty string, which is falsey. Also treat passing 'true'
    // the same as passing an empty string.
    var debug = (options.debug !== false);
    var debug_name_suffix;
    if (debug) {
        debug_name_suffix = (options.debug === true ? "" : options.debug);
    }

    var names_to_mangle = [];
    var unmangleable = [];
    var ignored = {};

    // step 1: find candidates to mangle
    ast.walk(new TreeWalker(function(node){
        if (node instanceof AST_ObjectKeyVal) {
            add(node.key, ignore_quoted && node.quote);
        }
        else if (node instanceof AST_ObjectProperty) {
            // setter or getter, since KeyVal is handled above
            add(node.key.name);
        }
        else if (node instanceof AST_Dot) {
            add(node.property);
        }
        else if (node instanceof AST_Sub) {
            addStrings(node.property, ignore_quoted);
        }
    }));

    // step 2: transform the tree, renaming properties
    return ast.transform(new TreeTransformer(function(node){
        if (node instanceof AST_ObjectKeyVal) {
            if (!(ignore_quoted && node.quote))
                node.key = mangle(node.key);
        }
        else if (node instanceof AST_ObjectProperty) {
            // setter or getter
            node.key.name = mangle(node.key.name);
        }
        else if (node instanceof AST_Dot) {
            node.property = mangle(node.property);
        }
        else if (node instanceof AST_Sub) {
            if (!ignore_quoted)
                node.property = mangleStrings(node.property);
        }
        // else if (node instanceof AST_String) {
        //     if (should_mangle(node.value)) {
        //         AST_Node.warn(
        //             "Found \"{prop}\" property candidate for mangling in an arbitrary string [{file}:{line},{col}]", {
        //                 file : node.start.file,
        //                 line : node.start.line,
        //                 col  : node.start.col,
        //                 prop : node.value
        //             }
        //         );
        //     }
        // }
    }));

    // only function declarations after this line

    function can_mangle(name) {
        if (!is_identifier(name)) return false;
        if (unmangleable.indexOf(name) >= 0) return false;
        if (reserved.indexOf(name) >= 0) return false;
        if (options.only_cache) {
            return cache.props.has(name);
        }
        if (/^[0-9.]+$/.test(name)) return false;
        return true;
    }

    function should_mangle(name) {
        if (ignore_quoted && name in ignored) return false;
        if (regex && !regex.test(name)) return false;
        if (reserved.indexOf(name) >= 0) return false;
        return cache.props.has(name)
            || names_to_mangle.indexOf(name) >= 0;
    }

    function add(name, ignore) {
        if (ignore) {
            ignored[name] = true;
            return;
        }

        if (can_mangle(name))
            push_uniq(names_to_mangle, name);

        if (!should_mangle(name)) {
            push_uniq(unmangleable, name);
        }
    }

    function mangle(name) {
        if (!should_mangle(name)) {
            return name;
        }

        var mangled = cache.props.get(name);
        if (!mangled) {
            if (debug) {
                // debug mode: use a prefix and suffix to preserve readability, e ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.merge"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>merge (obj, ext)](#apidoc.element.uglify-js.merge)
- description and source-code
```javascript
function merge(obj, ext) {
    var count = 0;
    for (var i in ext) if (HOP(ext, i)) {
        obj[i] = ext[i];
        count++;
    }
    return count;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.minify"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>minify (files, options)](#apidoc.element.uglify-js.minify)
- description and source-code
```javascript
minify = function (files, options) {
    options = UglifyJS.defaults(options, {
        spidermonkey     : false,
        outSourceMap     : null,
        outFileName      : null,
        sourceRoot       : null,
        inSourceMap      : null,
        sourceMapUrl     : null,
        sourceMapInline  : false,
        fromString       : false,
        warnings         : false,
        mangle           : {},
        mangleProperties : false,
        nameCache        : null,
        output           : null,
        compress         : {},
        parse            : {}
    });
    UglifyJS.base54.reset();

    var inMap = options.inSourceMap;
    if (typeof inMap == "string" && inMap != "inline") {
        inMap = JSON.parse(fs.readFileSync(inMap, "utf8"));
    }

    // 1. parse
    var toplevel = null,
        sourcesContent = {};

    if (options.spidermonkey) {
        if (inMap == "inline") {
            throw new Error("inline source map only works with built-in parser");
        }
        toplevel = UglifyJS.AST_Node.from_mozilla_ast(files);
    } else {
        function addFile(file, fileUrl) {
            var code = options.fromString
                ? file
                : fs.readFileSync(file, "utf8");
            if (inMap == "inline") {
                inMap = read_source_map(code);
            }
            sourcesContent[fileUrl] = code;
            toplevel = UglifyJS.parse(code, {
                filename: fileUrl,
                toplevel: toplevel,
                bare_returns: options.parse ? options.parse.bare_returns : undefined
            });
        }
        if (!options.fromString) {
            files = UglifyJS.simple_glob(files);
            if (inMap == "inline" && files.length > 1) {
                throw new Error("inline source map only works with singular input");
            }
        }
        [].concat(files).forEach(function (files, i) {
            if (typeof files === 'string') {
                addFile(files, options.fromString ? i : files);
            } else {
                for (var fileUrl in files) {
                    addFile(files[fileUrl], fileUrl);
                }
            }
        });
    }
    if (options.wrap) {
      toplevel = toplevel.wrap_commonjs(options.wrap, options.exportAll);
    }

    // 2. compress
    if (options.compress) {
        var compress = { warnings: options.warnings };
        UglifyJS.merge(compress, options.compress);
        toplevel.figure_out_scope(options.mangle);
        var sq = UglifyJS.Compressor(compress);
        toplevel = sq.compress(toplevel);
    }

    // 3. mangle properties
    if (options.mangleProperties || options.nameCache) {
        options.mangleProperties.cache = UglifyJS.readNameCache(options.nameCache, "props");
        toplevel = UglifyJS.mangle_properties(toplevel, options.mangleProperties);
        UglifyJS.writeNameCache(options.nameCache, "props", options.mangleProperties.cache);
    }

    // 4. mangle
    if (options.mangle) {
        toplevel.figure_out_scope(options.mangle);
        toplevel.compute_char_frequency(options.mangle);
        toplevel.mangle_names(options.mangle);
    }

    // 5. output
    var output = { max_line_len: 32000 };
    if (options.outSourceMap || options.sourceMapInline) {
        output.source_map = UglifyJS.SourceMap({
            // prefer outFileName, otherwise use outSourceMap without .map suffix
            file: options.outFileName || (typeof options.outSourceMap === 'string' ? options.outSourceMap.replace(/\.map$/i, '') :
null),
            orig: inMap,
            root: options.sourceRoot
        });
        if (options.sourceMapIncludeSources) {
            for (var file in sourcesContent) {
                if (sourcesContent.hasOwnProperty(file)) {
                    output.source_map.get().setSourceContent(file, sourcesContent[file]);
                }
            }
        }

    }
    if (options.output) {
        UglifyJS.merge(output, options.output);
    }
    var stream = UglifyJS.OutputStream(output);
    toplevel.print(stream);


    var source_map = output.source_ ...
```
- example usage
```shell
...
<a name="codegen-options"></a>

#### Conditional compilation, API
You can also use conditional compilation via the programmatic API. With the difference that the
property name is 'global_defs' and is a compressor property:

'''js
uglifyJS.minify([ "input.js"], {
    compress: {
        dead_code: true,
        global_defs: {
            DEBUG: false
        }
    }
});
...
```

#### <a name="apidoc.element.uglify-js.parse"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>parse ($TEXT, options)](#apidoc.element.uglify-js.parse)
- description and source-code
```javascript
function parse($TEXT, options) {

    options = defaults(options, {
        strict         : false,
        filename       : null,
        toplevel       : null,
        expression     : false,
        html5_comments : true,
        bare_returns   : false,
        shebang        : true,
        cli            : false,
    });

    var S = {
        input         : (typeof $TEXT == "string"
                         ? tokenizer($TEXT, options.filename,
                                     options.html5_comments, options.shebang)
                         : $TEXT),
        token         : null,
        prev          : null,
        peeked        : null,
        in_function   : 0,
        in_directives : true,
        in_loop       : 0,
        labels        : []
    };

    S.token = next();

    function is(type, value) {
        return is_token(S.token, type, value);
    };

    function peek() { return S.peeked || (S.peeked = S.input()); };

    function next() {
        S.prev = S.token;
        if (S.peeked) {
            S.token = S.peeked;
            S.peeked = null;
        } else {
            S.token = S.input();
        }
        S.in_directives = S.in_directives && (
            S.token.type == "string" || is("punc", ";")
        );
        return S.token;
    };

    function prev() {
        return S.prev;
    };

    function croak(msg, line, col, pos) {
        var ctx = S.input.context();
        js_error(msg,
                 ctx.filename,
                 line != null ? line : ctx.tokline,
                 col != null ? col : ctx.tokcol,
                 pos != null ? pos : ctx.tokpos);
    };

    function token_error(token, msg) {
        croak(msg, token.line, token.col);
    };

    function unexpected(token) {
        if (token == null)
            token = S.token;
        token_error(token, "Unexpected token: " + token.type + " (" + token.value + ")");
    };

    function expect_token(type, val) {
        if (is(type, val)) {
            return next();
        }
        token_error(S.token, "Unexpected token " + S.token.type + " «" + S.token.value + "»" + ", expected " + type + " «" + val
 + "»");
    };

    function expect(punc) { return expect_token("punc", punc); };

    function can_insert_semicolon() {
        return !options.strict && (
            S.token.nlb || is("eof") || is("punc", "}")
        );
    };

    function semicolon(optional) {
        if (is("punc", ";")) next();
        else if (!optional && !can_insert_semicolon()) unexpected();
    };

    function parenthesised() {
        expect("(");
        var exp = expression(true);
        expect(")");
        return exp;
    };

    function embed_tokens(parser) {
        return function() {
            var start = S.token;
            var expr = parser();
            var end = prev();
            expr.start = start;
            expr.end = end;
            return expr;
        };
    };

    function handle_regexp() {
        if (is("operator", "/") || is("operator", "/=")) {
            S.peeked = null;
            S.token = S.input(S.token.value.substr(1)); // force regexp
        }
    };

    var statement = embed_tokens(function() {
        var tmp;
        handle_regexp();
        switch (S.token.type) {
          case "string":
            var dir = false;
            if (S.in_directives === true) {
                if ((is_token(peek(), "punc", ";") || peek().nlb) && S.token.raw.indexOf("\\") === -1) {
                    S.input.add_directive(S.token.value);
                } else {
                    S.in_directives = false;
                }
            }
            var dir = S.in_directives, stat = simple_statement();
            if (dir) {
                return new AST_Directive({
                    start : stat.body.start,
                    end   : stat.body.end,
                    quote : stat.body.quote,
                    value : stat.body.value,
                });
            }
            return stat;
          case "num":
          case "regexp":
          case "operator":
          case "atom": ...
```
- example usage
```shell
...
'''

If your input source map is not in a file, you can pass it in as an object
using the 'inSourceMap' argument:

'''javascript
var result = UglifyJS.minify("compiled.js", {
	inSourceMap: JSON.parse(my_source_map_string),
	outSourceMap: "minified.js.map"
});
'''

The 'inSourceMap' is only used if you also request 'outSourceMap' (it makes
no sense otherwise).
...
```

#### <a name="apidoc.element.uglify-js.push_uniq"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>push_uniq (array, el)](#apidoc.element.uglify-js.push_uniq)
- description and source-code
```javascript
function push_uniq(array, el) {
    if (array.indexOf(el) < 0)
        array.push(el);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.readDefaultReservedFile"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>readDefaultReservedFile (reserved)](#apidoc.element.uglify-js.readDefaultReservedFile)
- description and source-code
```javascript
readDefaultReservedFile = function (reserved) {
    return readReservedFile(require.resolve("./domprops.json"), reserved);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.readNameCache"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>readNameCache (filename, key)](#apidoc.element.uglify-js.readNameCache)
- description and source-code
```javascript
readNameCache = function (filename, key) {
    var cache = null;
    if (filename) {
        try {
            var cache = fs.readFileSync(filename, "utf8");
            cache = JSON.parse(cache)[key];
            if (!cache) throw "init";
            cache.props = UglifyJS.Dictionary.fromObject(cache.props);
        } catch(ex) {
            cache = {
                cname: -1,
                props: new UglifyJS.Dictionary()
            };
        }
    }
    return cache;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.readReservedFile"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>readReservedFile (filename, reserved)](#apidoc.element.uglify-js.readReservedFile)
- description and source-code
```javascript
function readReservedFile(filename, reserved) {
    if (!reserved) {
        reserved = { vars: [], props: [] };
    }
    var data = fs.readFileSync(filename, "utf8");
    data = JSON.parse(data);
    if (data.vars) {
        data.vars.forEach(function(name){
            UglifyJS.push_uniq(reserved.vars, name);
        });
    }
    if (data.props) {
        data.props.forEach(function(name){
            UglifyJS.push_uniq(reserved.props, name);
        });
    }
    return reserved;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.simple_glob"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>simple_glob (glob)](#apidoc.element.uglify-js.simple_glob)
- description and source-code
```javascript
function simple_glob(glob) {
    if (Array.isArray(glob)) {
        return [].concat.apply([], glob.map(simple_glob));
    }
    if (glob.match(/\*|\?/)) {
        var dir = path.dirname(glob);
        try {
            var entries = fs.readdirSync(dir);
        } catch (ex) {}
        if (entries) {
            var pattern = "^" + path.basename(glob)
                .replace(/[.+^$[\]\\(){}]/g, "\\$&")
                .replace(/\*/g, "[^/\\\\]*")
                .replace(/\?/g, "[^/\\\\]") + "$";
            var mod = process.platform === "win32" ? "i" : "";
            var rx = new RegExp(pattern, mod);
            var results = entries.filter(function(name) {
                return rx.test(name);
            }).map(function(name) {
                return path.join(dir, name);
            });
            if (results.length) return results;
        }
    }
    return [ glob ];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.string_template"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>string_template (text, props)](#apidoc.element.uglify-js.string_template)
- description and source-code
```javascript
function string_template(text, props) {
    return text.replace(/\{(.+?)\}/g, function(str, p){
        return props && props[p];
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.tokenizer"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>tokenizer ($TEXT, filename, html5_comments, shebang)](#apidoc.element.uglify-js.tokenizer)
- description and source-code
```javascript
function tokenizer($TEXT, filename, html5_comments, shebang) {

    var S = {
        text            : $TEXT,
        filename        : filename,
        pos             : 0,
        tokpos          : 0,
        line            : 1,
        tokline         : 0,
        col             : 0,
        tokcol          : 0,
        newline_before  : false,
        regex_allowed   : false,
        comments_before : [],
        directives      : {},
        directive_stack : []
    };

    function peek() { return S.text.charAt(S.pos); };

    function next(signal_eof, in_string) {
        var ch = S.text.charAt(S.pos++);
        if (signal_eof && !ch)
            throw EX_EOF;
        if (NEWLINE_CHARS(ch)) {
            S.newline_before = S.newline_before || !in_string;
            ++S.line;
            S.col = 0;
            if (!in_string && ch == "\r" && peek() == "\n") {
                // treat a \r\n sequence as a single \n
                ++S.pos;
                ch = "\n";
            }
        } else {
            ++S.col;
        }
        return ch;
    };

    function forward(i) {
        while (i-- > 0) next();
    };

    function looking_at(str) {
        return S.text.substr(S.pos, str.length) == str;
    };

    function find_eol() {
        var text = S.text;
        for (var i = S.pos, n = S.text.length; i < n; ++i) {
            var ch = text[i];
            if (NEWLINE_CHARS(ch))
                return i;
        }
        return -1;
    };

    function find(what, signal_eof) {
        var pos = S.text.indexOf(what, S.pos);
        if (signal_eof && pos == -1) throw EX_EOF;
        return pos;
    };

    function start_token() {
        S.tokline = S.line;
        S.tokcol = S.col;
        S.tokpos = S.pos;
    };

    var prev_was_dot = false;
    function token(type, value, is_comment) {
        S.regex_allowed = ((type == "operator" && !UNARY_POSTFIX(value)) ||
                           (type == "keyword" && KEYWORDS_BEFORE_EXPRESSION(value)) ||
                           (type == "punc" && PUNC_BEFORE_EXPRESSION(value)));
        prev_was_dot = (type == "punc" && value == ".");
        var ret = {
            type    : type,
            value   : value,
            line    : S.tokline,
            col     : S.tokcol,
            pos     : S.tokpos,
            endline : S.line,
            endcol  : S.col,
            endpos  : S.pos,
            nlb     : S.newline_before,
            file    : filename
        };
        if (/^(?:num|string|regexp)$/i.test(type)) {
            ret.raw = $TEXT.substring(ret.pos, ret.endpos);
        }
        if (!is_comment) {
            ret.comments_before = S.comments_before;
            S.comments_before = [];
            // make note of any newlines in the comments that came before
            for (var i = 0, len = ret.comments_before.length; i < len; i++) {
                ret.nlb = ret.nlb || ret.comments_before[i].nlb;
            }
        }
        S.newline_before = false;
        return new AST_Token(ret);
    };

    function skip_whitespace() {
        while (WHITESPACE_CHARS(peek()))
            next();
    };

    function read_while(pred) {
        var ret = "", ch, i = 0;
        while ((ch = peek()) && pred(ch, i++))
            ret += next();
        return ret;
    };

    function parse_error(err) {
        js_error(err, filename, S.tokline, S.tokcol, S.tokpos);
    };

    function read_num(prefix) {
        var has_e = false, after_e = false, has_x = false, has_dot = prefix == ".";
        var num = read_while(function(ch, i){
            var code = ch.charCodeAt(0);
            switch (code) {
              case 120: case 88: // xX
                return has_x ? false : (has_x = true);
              case 101: case 69: // eE
                return has_x ? true : has_e ? false : (has_e = after_e = true);
              case 45: // -
                return after_e || (i == 0 && !prefix);
              case 43: // +
                return after_e;
              case (after_e = false, 46): // .
                return (!has_dot && !has_x && !ha ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.writeNameCache"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>writeNameCache (filename, key, cache)](#apidoc.element.uglify-js.writeNameCache)
- description and source-code
```javascript
writeNameCache = function (filename, key, cache) {
    if (filename) {
        var data;
        try {
            data = fs.readFileSync(filename, "utf8");
            data = JSON.parse(data);
        } catch(ex) {
            data = {};
        }
        data[key] = {
            cname: cache.cname,
            props: cache.props.toObject()
        };
        fs.writeFileSync(filename, JSON.stringify(data, null, 2), "utf8");
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Accessor"></a>[module uglify-js.AST_Accessor](#apidoc.module.uglify-js.AST_Accessor)

#### <a name="apidoc.element.uglify-js.AST_Accessor.AST_Accessor"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Accessor (props)](#apidoc.element.uglify-js.AST_Accessor.AST_Accessor)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Accessor.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>BASE (props)](#apidoc.element.uglify-js.AST_Accessor.BASE)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Accessor.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Accessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Accessor.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Accessor.prototype"></a>[module uglify-js.AST_Accessor.prototype](#apidoc.module.uglify-js.AST_Accessor.prototype)

#### <a name="apidoc.element.uglify-js.AST_Accessor.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Accessor.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Accessor.prototype.CTOR)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Array"></a>[module uglify-js.AST_Array](#apidoc.module.uglify-js.AST_Array)

#### <a name="apidoc.element.uglify-js.AST_Array.AST_Array"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Array (props)](#apidoc.element.uglify-js.AST_Array.AST_Array)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>BASE (props)](#apidoc.element.uglify-js.AST_Array.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Array.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Array.prototype"></a>[module uglify-js.AST_Array.prototype](#apidoc.module.uglify-js.AST_Array.prototype)

#### <a name="apidoc.element.uglify-js.AST_Array.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Array.prototype.CTOR)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Array.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.with_square(function(){
        var a = self.elements, len = a.length;
        if (len > 0) output.space();
        a.forEach(function(exp, i){
            if (i) output.comma();
            exp.print(output);
            // If the final element is a hole, we need to make sure it
            // doesn't look like a trailing comma, by inserting an actual
            // trailing comma.
            if (i === len - 1 && exp instanceof AST_Hole)
              output.comma();
        });
        if (len > 0) output.space();
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_Array.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    if (compressor.option("unsafe")) {
        return this.elements.map(function(element) {
            return ev(element, compressor);
        });
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Array.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        var elements = this.elements;
        for (var i = 0, len = elements.length; i < len; i++) {
            elements[i]._walk(visitor);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Array.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    var values = trim(this.elements, compressor, first_in_statement);
    return values && AST_Seq.from_array(values);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Array.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    for (var i = this.elements.length; --i >= 0;)
        if (this.elements[i].has_side_effects(compressor))
            return true;
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Array.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Array.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Array.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Array.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Array.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Assign"></a>[module uglify-js.AST_Assign](#apidoc.module.uglify-js.AST_Assign)

#### <a name="apidoc.element.uglify-js.AST_Assign.AST_Assign"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Assign (props)](#apidoc.element.uglify-js.AST_Assign.AST_Assign)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>BASE (props)](#apidoc.element.uglify-js.AST_Assign.BASE)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Assign.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Assign.prototype"></a>[module uglify-js.AST_Assign.prototype](#apidoc.module.uglify-js.AST_Assign.prototype)

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Assign.prototype.CTOR)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Assign.prototype.drop_side_effect_free)
- description and source-code
```javascript
function return_this() { return this; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Assign.prototype.has_side_effects)
- description and source-code
```javascript
function return_true() { return true; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Assign.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return this.operator == "=" && this.right.is_boolean();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.is_number"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Assign.prototype.is_number)
- description and source-code
```javascript
is_number = function (compressor){
    return assign(this.operator) || this.right.is_number(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Assign.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return (this.operator == "=" || this.operator == "+=") && this.right.is_string(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Assign.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    // !(a = false) → true
    if (p instanceof AST_Unary)
        return true;
    // 1 + (a = 2) + 3 → 6, side effect setting a = 2
    if (p instanceof AST_Binary && !(p instanceof AST_Assign))
        return true;
    // (a = func)() —or— new (a = Object)()
    if (p instanceof AST_Call && p.expression === this)
        return true;
    // (a = foo) ? bar : baz
    if (p instanceof AST_Conditional && p.condition === this)
        return true;
    // (a = foo)["prop"] —or— (a = foo).prop
    if (p instanceof AST_PropAccess && p.expression === this)
        return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Assign.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Assign.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Assign.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Assign.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Atom"></a>[module uglify-js.AST_Atom](#apidoc.module.uglify-js.AST_Atom)

#### <a name="apidoc.element.uglify-js.AST_Atom.AST_Atom"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Atom (props)](#apidoc.element.uglify-js.AST_Atom.AST_Atom)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>BASE (props)](#apidoc.element.uglify-js.AST_Atom.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Atom.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Atom.SUBCLASSES"></a>[module uglify-js.AST_Atom.SUBCLASSES](#apidoc.module.uglify-js.AST_Atom.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Atom.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.1)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.4)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Atom.SUBCLASSES.5)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Atom.prototype"></a>[module uglify-js.AST_Atom.prototype](#apidoc.module.uglify-js.AST_Atom.prototype)

#### <a name="apidoc.element.uglify-js.AST_Atom.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Atom.prototype.CTOR)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Atom.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Atom.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Atom.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Binary"></a>[module uglify-js.AST_Binary](#apidoc.module.uglify-js.AST_Binary)

#### <a name="apidoc.element.uglify-js.AST_Binary.AST_Binary"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Binary (props)](#apidoc.element.uglify-js.AST_Binary.AST_Binary)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>BASE (props)](#apidoc.element.uglify-js.AST_Binary.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Binary.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Binary.SUBCLASSES"></a>[module uglify-js.AST_Binary.SUBCLASSES](#apidoc.module.uglify-js.AST_Binary.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Binary.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Binary.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Binary.prototype"></a>[module uglify-js.AST_Binary.prototype](#apidoc.module.uglify-js.AST_Binary.prototype)

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Binary.prototype.CTOR)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Binary.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var op = self.operator;
    self.left.print(output);
    if (op[0] == ">"<span class="apidocCodeCommentSpan"> /* ">>" ">>>" ">" ">=" */
</span>        && self.left instanceof AST_UnaryPostfix
        && self.left.operator == "--") {
        // space is mandatory to avoid outputting -->
        output.print(" ");
    } else {
        // the space is optional depending on "beautify"
        output.space();
    }
    output.print(op);
    if ((op == "<" || op == "<<")
        && self.right instanceof AST_UnaryPrefix
        && self.right.operator == "!"
        && self.right.expression instanceof AST_UnaryPrefix
        && self.right.expression.operator == "--") {
        // space is mandatory to avoid outputting <!--
        output.print(" ");
    } else {
        // the space is optional depending on "beautify"
        output.space();
    }
    self.right.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>_eval (c)](#apidoc.element.uglify-js.AST_Binary.prototype._eval)
- description and source-code
```javascript
_eval = function (c){
    var left = this.left, right = this.right, result;
    switch (this.operator) {
      case "&&"  : result = ev(left, c) &&  ev(right, c); break;
      case "||"  : result = ev(left, c) ||  ev(right, c); break;
      case "|"   : result = ev(left, c) |   ev(right, c); break;
      case "&"   : result = ev(left, c) &   ev(right, c); break;
      case "^"   : result = ev(left, c) ^   ev(right, c); break;
      case "+"   : result = ev(left, c) +   ev(right, c); break;
      case "*"   : result = ev(left, c) *   ev(right, c); break;
      case "/"   : result = ev(left, c) /   ev(right, c); break;
      case "%"   : result = ev(left, c) %   ev(right, c); break;
      case "-"   : result = ev(left, c) -   ev(right, c); break;
      case "<<"  : result = ev(left, c) <<  ev(right, c); break;
      case ">>"  : result = ev(left, c) >>  ev(right, c); break;
      case ">>>" : result = ev(left, c) >>> ev(right, c); break;
      case "=="  : result = ev(left, c) ==  ev(right, c); break;
      case "===" : result = ev(left, c) === ev(right, c); break;
      case "!="  : result = ev(left, c) !=  ev(right, c); break;
      case "!==" : result = ev(left, c) !== ev(right, c); break;
      case "<"   : result = ev(left, c) <   ev(right, c); break;
      case "<="  : result = ev(left, c) <=  ev(right, c); break;
      case ">"   : result = ev(left, c) >   ev(right, c); break;
      case ">="  : result = ev(left, c) >=  ev(right, c); break;
      default:
          throw def;
    }
    if (isNaN(result) && c.find_parent(AST_With)) {
        // leave original expression as is
        throw def;
    }
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Binary.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.left._walk(visitor);
        this.right._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Binary.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    var right = this.right.drop_side_effect_free(compressor);
    if (!right) return this.left.drop_side_effect_free(compressor, first_in_statement);
    switch (this.operator) {
      case "&&":
      case "||":
        var node = this.clone();
        node.right = right;
        return node;
      default:
        var left = this.left.drop_side_effect_free(compressor, first_in_statement);
        if (!left) return this.right.drop_side_effect_free(compressor, first_in_statement);
        return make_node(AST_Seq, this, {
            car: left,
            cdr: right
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.left.has_side_effects(compressor)
        || this.right.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Binary.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return member(this.operator, binary_bool) ||
        ( (this.operator == "&&" || this.operator == "||") &&
          this.left.is_boolean() && this.right.is_boolean() );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.is_number"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.is_number)
- description and source-code
```javascript
is_number = function (compressor){
    return binary(this.operator) || this.operator == "+"
        && this.left.is_number(compressor)
        && this.right.is_number(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return this.operator == "+" &&
        (this.left.is_string(compressor) || this.right.is_string(compressor));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.lift_sequences"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.lift_sequences)
- description and source-code
```javascript
lift_sequences = function (compressor){
    if (compressor.option("sequences")) {
        if (this.left instanceof AST_Seq) {
            var seq = this.left;
            var x = seq.to_array();
            this.left = x.pop();
            x.push(this);
            return AST_Seq.from_array(x).optimize(compressor);
        }
        if (this.right instanceof AST_Seq && !this.left.has_side_effects(compressor)) {
            var assign = this.operator == "=" && this.left instanceof AST_SymbolRef;
            var root = this.right;
            var cursor, seq = root;
            while (assign || !seq.car.has_side_effects(compressor)) {
                cursor = seq;
                if (seq.cdr instanceof AST_Seq) {
                    seq = seq.cdr;
                } else break;
            }
            if (cursor) {
                this.right = cursor.cdr;
                cursor.cdr = this;
                return root.optimize(compressor);
            }
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Binary.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    // (foo && bar)()
    if (p instanceof AST_Call && p.expression === this)
        return true;
    // typeof (foo && bar)
    if (p instanceof AST_Unary)
        return true;
    // (foo && bar)["prop"], (foo && bar).prop
    if (p instanceof AST_PropAccess && p.expression === this)
        return true;
    // this deals with precedence: 3 * (2 + 1)
    if (p instanceof AST_Binary) {
        var po = p.operator, pp = PRECEDENCE[po];
        var so = this.operator, sp = PRECEDENCE[so];
        if (pp > sp
            || (pp == sp
                && this === p.right)) {
            return true;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Binary.prototype.negate)
- description and source-code
```javascript
negate = function (compressor, first_in_statement){
    return func.call(this, compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Binary.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Binary.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Binary.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Binary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Binary.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Block"></a>[module uglify-js.AST_Block](#apidoc.module.uglify-js.AST_Block)

#### <a name="apidoc.element.uglify-js.AST_Block.AST_Block"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Block (props)](#apidoc.element.uglify-js.AST_Block.AST_Block)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>BASE (props)](#apidoc.element.uglify-js.AST_Block.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Block.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Block.SUBCLASSES"></a>[module uglify-js.AST_Block.SUBCLASSES](#apidoc.module.uglify-js.AST_Block.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Block.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.0)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.3)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.4)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.5)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.SUBCLASSES.6"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.SUBCLASSES.</span>6 (props)](#apidoc.element.uglify-js.AST_Block.SUBCLASSES.6)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Block.prototype"></a>[module uglify-js.AST_Block.prototype](#apidoc.module.uglify-js.AST_Block.prototype)

#### <a name="apidoc.element.uglify-js.AST_Block.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Block.prototype.CTOR)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Block.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Block.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    for (var i = this.body.length; --i >= 0;) {
        if (this.body[i].has_side_effects(compressor))
            return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Block.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Block.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Block.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Block.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Block.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Block.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_BlockStatement"></a>[module uglify-js.AST_BlockStatement](#apidoc.module.uglify-js.AST_BlockStatement)

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.AST_BlockStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_BlockStatement (props)](#apidoc.element.uglify-js.AST_BlockStatement.AST_BlockStatement)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_BlockStatement.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_BlockStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_BlockStatement.prototype"></a>[module uglify-js.AST_BlockStatement.prototype](#apidoc.module.uglify-js.AST_BlockStatement.prototype)

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_BlockStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_BlockStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    print_bracketed(self.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_BlockStatement.prototype.aborts)
- description and source-code
```javascript
function block_aborts(){
    var n = this.body.length;
    return n > 0 && aborts(this.body[n - 1]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_BlockStatement.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_BlockStatement.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_BlockStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_BlockStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_BlockStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Boolean"></a>[module uglify-js.AST_Boolean](#apidoc.module.uglify-js.AST_Boolean)

#### <a name="apidoc.element.uglify-js.AST_Boolean.AST_Boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Boolean (props)](#apidoc.element.uglify-js.AST_Boolean.AST_Boolean)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Boolean.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>BASE (props)](#apidoc.element.uglify-js.AST_Boolean.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Boolean.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Boolean.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Boolean.SUBCLASSES"></a>[module uglify-js.AST_Boolean.SUBCLASSES](#apidoc.module.uglify-js.AST_Boolean.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Boolean.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Boolean.SUBCLASSES.0)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Boolean.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Boolean.SUBCLASSES.1)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Boolean.prototype"></a>[module uglify-js.AST_Boolean.prototype](#apidoc.module.uglify-js.AST_Boolean.prototype)

#### <a name="apidoc.element.uglify-js.AST_Boolean.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Boolean.prototype.CTOR)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Boolean.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Boolean.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Boolean.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Boolean.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Boolean.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Break"></a>[module uglify-js.AST_Break](#apidoc.module.uglify-js.AST_Break)

#### <a name="apidoc.element.uglify-js.AST_Break.AST_Break"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Break (props)](#apidoc.element.uglify-js.AST_Break.AST_Break)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Break.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>BASE (props)](#apidoc.element.uglify-js.AST_Break.BASE)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Break.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Break.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Break.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Break.prototype"></a>[module uglify-js.AST_Break.prototype](#apidoc.module.uglify-js.AST_Break.prototype)

#### <a name="apidoc.element.uglify-js.AST_Break.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Break.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Break.prototype.CTOR)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Break.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Break.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Break.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "break");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Break.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Break.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Break.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Call"></a>[module uglify-js.AST_Call](#apidoc.module.uglify-js.AST_Call)

#### <a name="apidoc.element.uglify-js.AST_Call.AST_Call"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Call (props)](#apidoc.element.uglify-js.AST_Call.AST_Call)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>BASE (props)](#apidoc.element.uglify-js.AST_Call.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Call.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Call.SUBCLASSES"></a>[module uglify-js.AST_Call.SUBCLASSES](#apidoc.module.uglify-js.AST_Call.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Call.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Call.SUBCLASSES.0)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Call.prototype"></a>[module uglify-js.AST_Call.prototype](#apidoc.module.uglify-js.AST_Call.prototype)

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Call.prototype.CTOR)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Call.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.expression.print(output);
    if (self instanceof AST_New && !need_constructor_parens(self, output))
        return;
    output.with_parens(function(){
        self.args.forEach(function(expr, i){
            if (i) output.comma();
            expr.print(output);
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Call.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        var args = this.args;
        for (var i = 0, len = args.length; i < len; i++) {
            args[i]._walk(visitor);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Call.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    if (!this.has_pure_annotation(compressor) && compressor.pure_funcs(this)) {
        if (this.expression instanceof AST_Function
            && (!this.expression.name || !this.expression.name.definition().references.length)) {
            var node = this.clone();
            node.expression = node.expression.process_expression(false);
            return node;
        }
        return this;
    }
    if (this.pure) {
        compressor.warn("Dropping __PURE__ call [{file}:{line},{col}]", this.start);
        this.pure.value = this.pure.value.replace(/[@#]__PURE__/g, ' ');
    }
    var args = trim(this.args, compressor, first_in_statement);
    return args && AST_Seq.from_array(args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.has_pure_annotation"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>has_pure_annotation (compressor)](#apidoc.element.uglify-js.AST_Call.prototype.has_pure_annotation)
- description and source-code
```javascript
has_pure_annotation = function (compressor) {
    if (!compressor.option("side_effects")) return false;
    if (this.pure !== undefined) return this.pure;
    var pure = false;
    var comments, last_comment;
    if (this.start
        && (comments = this.start.comments_before)
        && comments.length
        && /[@#]__PURE__/.test((last_comment = comments[comments.length - 1]).value)) {
        pure = last_comment;
    }
    return this.pure = pure;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Call.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    if (!this.has_pure_annotation(compressor) && compressor.pure_funcs(this)) return true;
    for (var i = this.args.length; --i >= 0;) {
        if (this.args[i].has_side_effects(compressor))
            return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Call.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent(), p1;
    if (p instanceof AST_New && p.expression === this)
        return true;

    // workaround for Safari bug.
    // https://bugs.webkit.org/show_bug.cgi?id=123506
    return this.expression instanceof AST_Function
        && p instanceof AST_PropAccess
        && p.expression === this
        && (p1 = output.parent(1)) instanceof AST_Assign
        && p1.left === p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Call.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Call.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Call.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Call.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Call.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Case"></a>[module uglify-js.AST_Case](#apidoc.module.uglify-js.AST_Case)

#### <a name="apidoc.element.uglify-js.AST_Case.AST_Case"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Case (props)](#apidoc.element.uglify-js.AST_Case.AST_Case)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Case.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>BASE (props)](#apidoc.element.uglify-js.AST_Case.BASE)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Case.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Case.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Case.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Case.prototype"></a>[module uglify-js.AST_Case.prototype](#apidoc.module.uglify-js.AST_Case.prototype)

#### <a name="apidoc.element.uglify-js.AST_Case.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Case.prototype.CTOR)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Case.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Case.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("case");
    output.space();
    self.expression.print(output);
    output.print(":");
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Case.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Case.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Case.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Case.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Case.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Case.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Case.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Catch"></a>[module uglify-js.AST_Catch](#apidoc.module.uglify-js.AST_Catch)

#### <a name="apidoc.element.uglify-js.AST_Catch.AST_Catch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Catch (props)](#apidoc.element.uglify-js.AST_Catch.AST_Catch)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Catch.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>BASE (props)](#apidoc.element.uglify-js.AST_Catch.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Catch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Catch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Catch.prototype"></a>[module uglify-js.AST_Catch.prototype](#apidoc.module.uglify-js.AST_Catch.prototype)

#### <a name="apidoc.element.uglify-js.AST_Catch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Catch.prototype.CTOR)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Catch.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Catch.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("catch");
    output.space();
    output.with_parens(function(){
        self.argname.print(output);
    });
    output.space();
    print_bracketed(self.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Catch.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Catch.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.argname._walk(visitor);
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Catch.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Catch.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Catch.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Catch.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Catch.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Catch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Catch.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Conditional"></a>[module uglify-js.AST_Conditional](#apidoc.module.uglify-js.AST_Conditional)

#### <a name="apidoc.element.uglify-js.AST_Conditional.AST_Conditional"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Conditional (props)](#apidoc.element.uglify-js.AST_Conditional.AST_Conditional)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>BASE (props)](#apidoc.element.uglify-js.AST_Conditional.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Conditional.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Conditional.prototype"></a>[module uglify-js.AST_Conditional.prototype](#apidoc.module.uglify-js.AST_Conditional.prototype)

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Conditional.prototype.CTOR)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Conditional.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.condition.print(output);
    output.space();
    output.print("?");
    output.space();
    self.consequent.print(output);
    output.space();
    output.colon();
    self.alternative.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    return ev(this.condition, compressor)
        ? ev(this.consequent, compressor)
        : ev(this.alternative, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Conditional.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.condition._walk(visitor);
        this.consequent._walk(visitor);
        this.alternative._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>drop_side_effect_free (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor){
    var consequent = this.consequent.drop_side_effect_free(compressor);
    var alternative = this.alternative.drop_side_effect_free(compressor);
    if (consequent === this.consequent && alternative === this.alternative) return this;
    if (!consequent) return alternative ? make_node(AST_Binary, this, {
        operator: "||",
        left: this.condition,
        right: alternative
    }) : this.condition.drop_side_effect_free(compressor);
    if (!alternative) return make_node(AST_Binary, this, {
        operator: "&&",
        left: this.condition,
        right: consequent
    });
    var node = this.clone();
    node.consequent = consequent;
    node.alternative = alternative;
    return node;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.condition.has_side_effects(compressor)
        || this.consequent.has_side_effects(compressor)
        || this.alternative.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Conditional.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return this.consequent.is_boolean() && this.alternative.is_boolean();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.is_number"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.is_number)
- description and source-code
```javascript
is_number = function (compressor){
    return this.consequent.is_number(compressor) && this.alternative.is_number(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return this.consequent.is_string(compressor) && this.alternative.is_string(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Conditional.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    // !(a = false) → true
    if (p instanceof AST_Unary)
        return true;
    // 1 + (a = 2) + 3 → 6, side effect setting a = 2
    if (p instanceof AST_Binary && !(p instanceof AST_Assign))
        return true;
    // (a = func)() —or— new (a = Object)()
    if (p instanceof AST_Call && p.expression === this)
        return true;
    // (a = foo) ? bar : baz
    if (p instanceof AST_Conditional && p.condition === this)
        return true;
    // (a = foo)["prop"] —or— (a = foo).prop
    if (p instanceof AST_PropAccess && p.expression === this)
        return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Conditional.prototype.negate)
- description and source-code
```javascript
negate = function (compressor, first_in_statement){
    return func.call(this, compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Conditional.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Conditional.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Conditional.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Conditional.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Conditional.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Const"></a>[module uglify-js.AST_Const](#apidoc.module.uglify-js.AST_Const)

#### <a name="apidoc.element.uglify-js.AST_Const.AST_Const"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Const (props)](#apidoc.element.uglify-js.AST_Const.AST_Const)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Const.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>BASE (props)](#apidoc.element.uglify-js.AST_Const.BASE)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Const.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Const.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Const.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Const.prototype"></a>[module uglify-js.AST_Const.prototype](#apidoc.module.uglify-js.AST_Const.prototype)

#### <a name="apidoc.element.uglify-js.AST_Const.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Const.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Const.prototype.CTOR)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Const.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Const.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Const.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "const");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Constant"></a>[module uglify-js.AST_Constant](#apidoc.module.uglify-js.AST_Constant)

#### <a name="apidoc.element.uglify-js.AST_Constant.AST_Constant"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Constant (props)](#apidoc.element.uglify-js.AST_Constant.AST_Constant)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>BASE (props)](#apidoc.element.uglify-js.AST_Constant.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Constant.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Constant.SUBCLASSES"></a>[module uglify-js.AST_Constant.SUBCLASSES](#apidoc.module.uglify-js.AST_Constant.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Constant.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.0)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.literal = props.literal;this.value =
props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.2)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Constant.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Constant.prototype"></a>[module uglify-js.AST_Constant.prototype](#apidoc.module.uglify-js.AST_Constant.prototype)

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Constant.prototype.CTOR)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Constant.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print(self.getValue());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Constant.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    return this.getValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Constant.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Constant.prototype.drop_side_effect_free)
- description and source-code
```javascript
function return_null() { return null; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype.getValue"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>getValue ()](#apidoc.element.uglify-js.AST_Constant.prototype.getValue)
- description and source-code
```javascript
getValue = function () {
    return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Constant.prototype.has_side_effects)
- description and source-code
```javascript
function return_false() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Constant.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Constant.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Constant.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Continue"></a>[module uglify-js.AST_Continue](#apidoc.module.uglify-js.AST_Continue)

#### <a name="apidoc.element.uglify-js.AST_Continue.AST_Continue"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Continue (props)](#apidoc.element.uglify-js.AST_Continue.AST_Continue)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Continue.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>BASE (props)](#apidoc.element.uglify-js.AST_Continue.BASE)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Continue.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Continue.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Continue.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Continue.prototype"></a>[module uglify-js.AST_Continue.prototype](#apidoc.module.uglify-js.AST_Continue.prototype)

#### <a name="apidoc.element.uglify-js.AST_Continue.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Continue.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Continue.prototype.CTOR)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Continue.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Continue.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Continue.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "continue");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Continue.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Continue.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Continue.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_DWLoop"></a>[module uglify-js.AST_DWLoop](#apidoc.module.uglify-js.AST_DWLoop)

#### <a name="apidoc.element.uglify-js.AST_DWLoop.AST_DWLoop"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_DWLoop (props)](#apidoc.element.uglify-js.AST_DWLoop.AST_DWLoop)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_DWLoop.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>BASE (props)](#apidoc.element.uglify-js.AST_DWLoop.BASE)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_DWLoop.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_DWLoop.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_DWLoop.SUBCLASSES"></a>[module uglify-js.AST_DWLoop.SUBCLASSES](#apidoc.module.uglify-js.AST_DWLoop.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_DWLoop.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_DWLoop.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_DWLoop.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_DWLoop.SUBCLASSES.1)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_DWLoop.prototype"></a>[module uglify-js.AST_DWLoop.prototype](#apidoc.module.uglify-js.AST_DWLoop.prototype)

#### <a name="apidoc.element.uglify-js.AST_DWLoop.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_DWLoop.prototype.CTOR)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_DWLoop.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_DWLoop.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_DWLoop.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_DWLoop.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_DWLoop.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Debugger"></a>[module uglify-js.AST_Debugger](#apidoc.module.uglify-js.AST_Debugger)

#### <a name="apidoc.element.uglify-js.AST_Debugger.AST_Debugger"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Debugger (props)](#apidoc.element.uglify-js.AST_Debugger.AST_Debugger)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Debugger.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>BASE (props)](#apidoc.element.uglify-js.AST_Debugger.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Debugger.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Debugger.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Debugger.prototype"></a>[module uglify-js.AST_Debugger.prototype](#apidoc.module.uglify-js.AST_Debugger.prototype)

#### <a name="apidoc.element.uglify-js.AST_Debugger.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Debugger.prototype.CTOR)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Debugger.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Debugger.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("debugger");
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Debugger.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Debugger.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Debugger.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Debugger.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Debugger.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Debugger.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Debugger.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Default"></a>[module uglify-js.AST_Default](#apidoc.module.uglify-js.AST_Default)

#### <a name="apidoc.element.uglify-js.AST_Default.AST_Default"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Default (props)](#apidoc.element.uglify-js.AST_Default.AST_Default)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Default.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>BASE (props)](#apidoc.element.uglify-js.AST_Default.BASE)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Default.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Default.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Default.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Default.prototype"></a>[module uglify-js.AST_Default.prototype](#apidoc.module.uglify-js.AST_Default.prototype)

#### <a name="apidoc.element.uglify-js.AST_Default.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Default.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Default.prototype.CTOR)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Default.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Default.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Default.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("default:");
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Definitions"></a>[module uglify-js.AST_Definitions](#apidoc.module.uglify-js.AST_Definitions)

#### <a name="apidoc.element.uglify-js.AST_Definitions.AST_Definitions"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Definitions (props)](#apidoc.element.uglify-js.AST_Definitions.AST_Definitions)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>BASE (props)](#apidoc.element.uglify-js.AST_Definitions.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Definitions.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Definitions.SUBCLASSES"></a>[module uglify-js.AST_Definitions.SUBCLASSES](#apidoc.module.uglify-js.AST_Definitions.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Definitions.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Definitions.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Definitions.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Definitions.prototype"></a>[module uglify-js.AST_Definitions.prototype](#apidoc.module.uglify-js.AST_Definitions.prototype)

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Definitions.prototype.CTOR)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>_do_print (output, kind)](#apidoc.element.uglify-js.AST_Definitions.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, kind){
    output.print(kind);
    output.space();
    this.definitions.forEach(function(def, i){
        if (i) output.comma();
        def.print(output);
    });
    var p = output.parent();
    var in_for = p instanceof AST_For || p instanceof AST_ForIn;
    var avoid_semicolon = in_for && p.init === this;
    if (!avoid_semicolon)
        output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Definitions.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        var definitions = this.definitions;
        for (var i = 0, len = definitions.length; i < len; i++) {
            definitions[i]._walk(visitor);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Definitions.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Definitions.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype.remove_initializers"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>remove_initializers ()](#apidoc.element.uglify-js.AST_Definitions.prototype.remove_initializers)
- description and source-code
```javascript
remove_initializers = function (){
    this.definitions.forEach(function(def){ def.value = null });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype.to_assignments"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>to_assignments (compressor)](#apidoc.element.uglify-js.AST_Definitions.prototype.to_assignments)
- description and source-code
```javascript
to_assignments = function (compressor){
    var reduce_vars = compressor.option("reduce_vars");
    var assignments = this.definitions.reduce(function(a, def){
        if (def.value) {
            var name = make_node(AST_SymbolRef, def.name, def.name);
            a.push(make_node(AST_Assign, def, {
                operator : "=",
                left     : name,
                right    : def.value
            }));
            if (reduce_vars) name.definition().fixed = false;
        }
        return a;
    }, []);
    if (assignments.length == 0) return null;
    return AST_Seq.from_array(assignments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Definitions.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Definitions.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Definitions.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Definitions.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Defun"></a>[module uglify-js.AST_Defun](#apidoc.module.uglify-js.AST_Defun)

#### <a name="apidoc.element.uglify-js.AST_Defun.AST_Defun"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Defun (props)](#apidoc.element.uglify-js.AST_Defun.AST_Defun)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Defun.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>BASE (props)](#apidoc.element.uglify-js.AST_Defun.BASE)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Defun.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Defun.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Defun.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Defun.prototype"></a>[module uglify-js.AST_Defun.prototype](#apidoc.module.uglify-js.AST_Defun.prototype)

#### <a name="apidoc.element.uglify-js.AST_Defun.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Defun.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Defun.prototype.CTOR)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Defun.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Defun.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Defun.prototype.has_side_effects)
- description and source-code
```javascript
function return_true() { return true; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Defun.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Defun.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Defun.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Directive"></a>[module uglify-js.AST_Directive](#apidoc.module.uglify-js.AST_Directive)

#### <a name="apidoc.element.uglify-js.AST_Directive.AST_Directive"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Directive (props)](#apidoc.element.uglify-js.AST_Directive.AST_Directive)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Directive.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>BASE (props)](#apidoc.element.uglify-js.AST_Directive.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Directive.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Directive.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Directive.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Directive.prototype"></a>[module uglify-js.AST_Directive.prototype](#apidoc.module.uglify-js.AST_Directive.prototype)

#### <a name="apidoc.element.uglify-js.AST_Directive.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Directive.prototype.CTOR)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Directive.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Directive.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print_string(self.value, self.quote);
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Directive.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Directive.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Directive.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Directive.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Directive.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Directive.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Directive.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Do"></a>[module uglify-js.AST_Do](#apidoc.module.uglify-js.AST_Do)

#### <a name="apidoc.element.uglify-js.AST_Do.AST_Do"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Do (props)](#apidoc.element.uglify-js.AST_Do.AST_Do)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Do.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>BASE (props)](#apidoc.element.uglify-js.AST_Do.BASE)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Do.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Do.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Do.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Do.prototype"></a>[module uglify-js.AST_Do.prototype](#apidoc.module.uglify-js.AST_Do.prototype)

#### <a name="apidoc.element.uglify-js.AST_Do.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Do.prototype.CTOR)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Do.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Do.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("do");
    output.space();
    make_block(self.body, output);
    output.space();
    output.print("while");
    output.space();
    output.with_parens(function(){
        self.condition.print(output);
    });
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Do.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Do.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.body._walk(visitor);
        this.condition._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Do.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Do.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Do.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Dot"></a>[module uglify-js.AST_Dot](#apidoc.module.uglify-js.AST_Dot)

#### <a name="apidoc.element.uglify-js.AST_Dot.AST_Dot"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Dot (props)](#apidoc.element.uglify-js.AST_Dot.AST_Dot)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>BASE (props)](#apidoc.element.uglify-js.AST_Dot.BASE)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Dot.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Dot.prototype"></a>[module uglify-js.AST_Dot.prototype](#apidoc.module.uglify-js.AST_Dot.prototype)

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Dot.prototype.CTOR)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Dot.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var expr = self.expression;
    expr.print(output);
    if (expr instanceof AST_Number && expr.getValue() >= 0) {
        if (!/[xa-f.)]/i.test(output.last())) {
            output.print(".");
        }
    }
    output.print(".");
    // the name after dot would be mapped about here.
    output.add_mapping(self.end);
    output.print_name(self.property);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype._find_defs"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>_find_defs (compressor, suffix)](#apidoc.element.uglify-js.AST_Dot.prototype._find_defs)
- description and source-code
```javascript
_find_defs = function (compressor, suffix){
    return this.expression._find_defs(compressor, suffix + "." + this.property);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Dot.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Dot.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    if (!compressor.option("pure_getters")) return this;
    return this.expression.drop_side_effect_free(compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Dot.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    if (!compressor.option("pure_getters")) return true;
    return this.expression.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Dot.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Dot.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Dot.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Dot.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_EmptyStatement"></a>[module uglify-js.AST_EmptyStatement](#apidoc.module.uglify-js.AST_EmptyStatement)

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.AST_EmptyStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_EmptyStatement (props)](#apidoc.element.uglify-js.AST_EmptyStatement.AST_EmptyStatement)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_EmptyStatement.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_EmptyStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_EmptyStatement.prototype"></a>[module uglify-js.AST_EmptyStatement.prototype](#apidoc.module.uglify-js.AST_EmptyStatement.prototype)

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_EmptyStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_EmptyStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_EmptyStatement.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_EmptyStatement.prototype.has_side_effects)
- description and source-code
```javascript
function return_false() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_EmptyStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_EmptyStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_EmptyStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Exit"></a>[module uglify-js.AST_Exit](#apidoc.module.uglify-js.AST_Exit)

#### <a name="apidoc.element.uglify-js.AST_Exit.AST_Exit"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Exit (props)](#apidoc.element.uglify-js.AST_Exit.AST_Exit)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Exit.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>BASE (props)](#apidoc.element.uglify-js.AST_Exit.BASE)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Exit.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Exit.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Exit.SUBCLASSES"></a>[module uglify-js.AST_Exit.SUBCLASSES](#apidoc.module.uglify-js.AST_Exit.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Exit.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Exit.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Exit.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Exit.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Exit.prototype"></a>[module uglify-js.AST_Exit.prototype](#apidoc.module.uglify-js.AST_Exit.prototype)

#### <a name="apidoc.element.uglify-js.AST_Exit.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Exit.prototype.CTOR)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Exit.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>_do_print (output, kind)](#apidoc.element.uglify-js.AST_Exit.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, kind){
    output.print(kind);
    if (this.value) {
        output.space();
        this.value.print(output);
    }
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Exit.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Exit.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, this.value && function(){
        this.value._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Exit.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Exit.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Exit.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_False"></a>[module uglify-js.AST_False](#apidoc.module.uglify-js.AST_False)

#### <a name="apidoc.element.uglify-js.AST_False.AST_False"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_False (props)](#apidoc.element.uglify-js.AST_False.AST_False)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_False.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_False.</span>BASE (props)](#apidoc.element.uglify-js.AST_False.BASE)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_False.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_False.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_False.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_False.prototype"></a>[module uglify-js.AST_False.prototype](#apidoc.module.uglify-js.AST_False.prototype)

#### <a name="apidoc.element.uglify-js.AST_False.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_False.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_False.prototype.CTOR)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_False.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_False.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_False.prototype.is_boolean)
- description and source-code
```javascript
function return_true() { return true; }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Finally"></a>[module uglify-js.AST_Finally](#apidoc.module.uglify-js.AST_Finally)

#### <a name="apidoc.element.uglify-js.AST_Finally.AST_Finally"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Finally (props)](#apidoc.element.uglify-js.AST_Finally.AST_Finally)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Finally.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>BASE (props)](#apidoc.element.uglify-js.AST_Finally.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Finally.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Finally.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Finally.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Finally.prototype"></a>[module uglify-js.AST_Finally.prototype](#apidoc.module.uglify-js.AST_Finally.prototype)

#### <a name="apidoc.element.uglify-js.AST_Finally.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Finally.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Finally.prototype.CTOR)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Finally.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Finally.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Finally.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("finally");
    output.space();
    print_bracketed(self.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Finally.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Finally.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Finally.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_For"></a>[module uglify-js.AST_For](#apidoc.module.uglify-js.AST_For)

#### <a name="apidoc.element.uglify-js.AST_For.AST_For"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_For (props)](#apidoc.element.uglify-js.AST_For.AST_For)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_For.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.</span>BASE (props)](#apidoc.element.uglify-js.AST_For.BASE)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_For.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_For.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_For.prototype"></a>[module uglify-js.AST_For.prototype](#apidoc.module.uglify-js.AST_For.prototype)

#### <a name="apidoc.element.uglify-js.AST_For.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_For.prototype.CTOR)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_For.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_For.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("for");
    output.space();
    output.with_parens(function(){
        if (self.init) {
            if (self.init instanceof AST_Definitions) {
                self.init.print(output);
            } else {
                parenthesize_for_noin(self.init, output, true);
            }
            output.print(";");
            output.space();
        } else {
            output.print(";");
        }
        if (self.condition) {
            self.condition.print(output);
            output.print(";");
            output.space();
        } else {
            output.print(";");
        }
        if (self.step) {
            self.step.print(output);
        }
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_For.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_For.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        if (this.init) this.init._walk(visitor);
        if (this.condition) this.condition._walk(visitor);
        if (this.step) this.step._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_For.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_For.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_For.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_For.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_For.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_For.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_For.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_ForIn"></a>[module uglify-js.AST_ForIn](#apidoc.module.uglify-js.AST_ForIn)

#### <a name="apidoc.element.uglify-js.AST_ForIn.AST_ForIn"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ForIn (props)](#apidoc.element.uglify-js.AST_ForIn.AST_ForIn)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ForIn.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>BASE (props)](#apidoc.element.uglify-js.AST_ForIn.BASE)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ForIn.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ForIn.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ForIn.prototype"></a>[module uglify-js.AST_ForIn.prototype](#apidoc.module.uglify-js.AST_ForIn.prototype)

#### <a name="apidoc.element.uglify-js.AST_ForIn.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ForIn.prototype.CTOR)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ForIn.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ForIn.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("for");
    output.space();
    output.with_parens(function(){
        self.init.print(output);
        output.space();
        output.print("in");
        output.space();
        self.object.print(output);
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ForIn.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_ForIn.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.init._walk(visitor);
        this.object._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ForIn.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_ForIn.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_ForIn.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ForIn.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_ForIn.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Function"></a>[module uglify-js.AST_Function](#apidoc.module.uglify-js.AST_Function)

#### <a name="apidoc.element.uglify-js.AST_Function.AST_Function"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Function (props)](#apidoc.element.uglify-js.AST_Function.AST_Function)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>BASE (props)](#apidoc.element.uglify-js.AST_Function.BASE)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Function.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Function.prototype"></a>[module uglify-js.AST_Function.prototype](#apidoc.module.uglify-js.AST_Function.prototype)

#### <a name="apidoc.element.uglify-js.AST_Function.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Function.prototype.CTOR)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Function.prototype.drop_side_effect_free)
- description and source-code
```javascript
function return_null() { return null; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Function.prototype.has_side_effects)
- description and source-code
```javascript
function return_false() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Function.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    if (first_in_statement(output)) {
        return true;
    }

    if (output.option('wrap_iife')) {
        var p = output.parent();
        return p instanceof AST_Call && p.expression === this;
    }

    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Function.prototype.negate)
- description and source-code
```javascript
negate = function (compressor, first_in_statement){
    return func.call(this, compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.prototype.next_mangled"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>next_mangled (options, def)](#apidoc.element.uglify-js.AST_Function.prototype.next_mangled)
- description and source-code
```javascript
next_mangled = function (options, def){
    // #179, #326
    // in Safari strict mode, something like (function x(x){...}) is a syntax error;
    // a function expression's argument cannot shadow the function expression's name

    var tricky_def = def.orig[0] instanceof AST_SymbolFunarg && this.name && this.name.definition();

    // the function's mangled_name is null when keep_fnames is true
    var tricky_name = tricky_def ? tricky_def.mangled_name || tricky_def.name : null;

    while (true) {
        var name = AST_Lambda.prototype.next_mangled.call(this, options, def);
        if (!tricky_name || tricky_name != name)
            return name;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Function.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Function.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Function.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Hole"></a>[module uglify-js.AST_Hole](#apidoc.module.uglify-js.AST_Hole)

#### <a name="apidoc.element.uglify-js.AST_Hole.AST_Hole"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Hole (props)](#apidoc.element.uglify-js.AST_Hole.AST_Hole)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Hole.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>BASE (props)](#apidoc.element.uglify-js.AST_Hole.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Hole.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Hole.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Hole.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Hole.prototype"></a>[module uglify-js.AST_Hole.prototype](#apidoc.module.uglify-js.AST_Hole.prototype)

#### <a name="apidoc.element.uglify-js.AST_Hole.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Hole.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Hole.prototype.CTOR)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Hole.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Hole.prototype.</span>_codegen ()](#apidoc.element.uglify-js.AST_Hole.prototype._codegen)
- description and source-code
```javascript
function noop() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Hole.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Hole.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Hole.prototype.to_mozilla_ast)
- description and source-code
```javascript
function To_Moz_ArrayHole() { return null }
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_If"></a>[module uglify-js.AST_If](#apidoc.module.uglify-js.AST_If)

#### <a name="apidoc.element.uglify-js.AST_If.AST_If"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_If (props)](#apidoc.element.uglify-js.AST_If.AST_If)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.</span>BASE (props)](#apidoc.element.uglify-js.AST_If.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_If.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_If.prototype"></a>[module uglify-js.AST_If.prototype](#apidoc.module.uglify-js.AST_If.prototype)

#### <a name="apidoc.element.uglify-js.AST_If.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_If.prototype.CTOR)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_If.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("if");
    output.space();
    output.with_parens(function(){
        self.condition.print(output);
    });
    output.space();
    if (self.alternative) {
        make_then(self, output);
        output.space();
        output.print("else");
        output.space();
        if (self.alternative instanceof AST_If)
            self.alternative.print(output);
        else
            force_statement(self.alternative, output);
    } else {
        self._do_print_body(output);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_If.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.condition._walk(visitor);
        this.body._walk(visitor);
        if (this.alternative) this.alternative._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_If.prototype.aborts)
- description and source-code
```javascript
aborts = function (){
    return this.alternative && aborts(this.body) && aborts(this.alternative) && this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_If.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_If.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_If.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_If.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_If.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_If.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Infinity"></a>[module uglify-js.AST_Infinity](#apidoc.module.uglify-js.AST_Infinity)

#### <a name="apidoc.element.uglify-js.AST_Infinity.AST_Infinity"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Infinity (props)](#apidoc.element.uglify-js.AST_Infinity.AST_Infinity)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Infinity.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>BASE (props)](#apidoc.element.uglify-js.AST_Infinity.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Infinity.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Infinity.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Infinity.prototype"></a>[module uglify-js.AST_Infinity.prototype](#apidoc.module.uglify-js.AST_Infinity.prototype)

#### <a name="apidoc.element.uglify-js.AST_Infinity.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Infinity.prototype.CTOR)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Infinity.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Infinity.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("Infinity");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Infinity.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Infinity.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Infinity.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_IterationStatement"></a>[module uglify-js.AST_IterationStatement](#apidoc.module.uglify-js.AST_IterationStatement)

#### <a name="apidoc.element.uglify-js.AST_IterationStatement.AST_IterationStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_IterationStatement (props)](#apidoc.element.uglify-js.AST_IterationStatement.AST_IterationStatement)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_IterationStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_IterationStatement.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_IterationStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_IterationStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_IterationStatement.SUBCLASSES"></a>[module uglify-js.AST_IterationStatement.SUBCLASSES](#apidoc.module.uglify-js.AST_IterationStatement.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.0)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.1)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_IterationStatement.SUBCLASSES.2)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_IterationStatement.prototype"></a>[module uglify-js.AST_IterationStatement.prototype](#apidoc.module.uglify-js.AST_IterationStatement.prototype)

#### <a name="apidoc.element.uglify-js.AST_IterationStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_IterationStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_IterationStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Jump"></a>[module uglify-js.AST_Jump](#apidoc.module.uglify-js.AST_Jump)

#### <a name="apidoc.element.uglify-js.AST_Jump.AST_Jump"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Jump (props)](#apidoc.element.uglify-js.AST_Jump.AST_Jump)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Jump.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>BASE (props)](#apidoc.element.uglify-js.AST_Jump.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Jump.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Jump.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Jump.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Jump.SUBCLASSES"></a>[module uglify-js.AST_Jump.SUBCLASSES](#apidoc.module.uglify-js.AST_Jump.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Jump.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Jump.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Jump.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Jump.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Jump.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Jump.SUBCLASSES.1)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Jump.prototype"></a>[module uglify-js.AST_Jump.prototype](#apidoc.module.uglify-js.AST_Jump.prototype)

#### <a name="apidoc.element.uglify-js.AST_Jump.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Jump.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Jump.prototype.CTOR)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Jump.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Jump.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_Jump.prototype.aborts)
- description and source-code
```javascript
function return_this() { return this; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Jump.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Jump.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Jump.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Label"></a>[module uglify-js.AST_Label](#apidoc.module.uglify-js.AST_Label)

#### <a name="apidoc.element.uglify-js.AST_Label.AST_Label"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Label (props)](#apidoc.element.uglify-js.AST_Label.AST_Label)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Label.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>BASE (props)](#apidoc.element.uglify-js.AST_Label.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Label.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Label.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Label.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Label.prototype"></a>[module uglify-js.AST_Label.prototype](#apidoc.module.uglify-js.AST_Label.prototype)

#### <a name="apidoc.element.uglify-js.AST_Label.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Label.prototype.CTOR)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Label.prototype.initialize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>initialize ()](#apidoc.element.uglify-js.AST_Label.prototype.initialize)
- description and source-code
```javascript
initialize = function () {
    this.references = [];
    this.thedef = this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Label.prototype.undeclared"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>undeclared ()](#apidoc.element.uglify-js.AST_Label.prototype.undeclared)
- description and source-code
```javascript
undeclared = function (){
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Label.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Label.prototype.</span>unmangleable ()](#apidoc.element.uglify-js.AST_Label.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (){
    return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_LabelRef"></a>[module uglify-js.AST_LabelRef](#apidoc.module.uglify-js.AST_LabelRef)

#### <a name="apidoc.element.uglify-js.AST_LabelRef.AST_LabelRef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabelRef (props)](#apidoc.element.uglify-js.AST_LabelRef.AST_LabelRef)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabelRef.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>BASE (props)](#apidoc.element.uglify-js.AST_LabelRef.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabelRef.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_LabelRef.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_LabelRef.prototype"></a>[module uglify-js.AST_LabelRef.prototype](#apidoc.module.uglify-js.AST_LabelRef.prototype)

#### <a name="apidoc.element.uglify-js.AST_LabelRef.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_LabelRef.prototype.CTOR)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabelRef.prototype.undeclared"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabelRef.prototype.</span>undeclared ()](#apidoc.element.uglify-js.AST_LabelRef.prototype.undeclared)
- description and source-code
```javascript
undeclared = function (){
    return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_LabeledStatement"></a>[module uglify-js.AST_LabeledStatement](#apidoc.module.uglify-js.AST_LabeledStatement)

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.AST_LabeledStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_LabeledStatement (props)](#apidoc.element.uglify-js.AST_LabeledStatement.AST_LabeledStatement)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_LabeledStatement.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_LabeledStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_LabeledStatement.prototype"></a>[module uglify-js.AST_LabeledStatement.prototype](#apidoc.module.uglify-js.AST_LabeledStatement.prototype)

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.label.print(output);
    output.colon();
    self.body.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.label._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype.clone"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>clone (deep)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.clone)
- description and source-code
```javascript
clone = function (deep) {
    var node = this._clone(deep);
    if (deep) {
        var refs = node.label.references;
        var label = this.label;
        node.walk(new TreeWalker(function(node) {
            if (node instanceof AST_LoopControl
                && node.label && node.label.thedef === label) {
                refs.push(node);
            }
        }));
    }
    return node;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_LabeledStatement.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LabeledStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_LabeledStatement.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Lambda"></a>[module uglify-js.AST_Lambda](#apidoc.module.uglify-js.AST_Lambda)

#### <a name="apidoc.element.uglify-js.AST_Lambda.AST_Lambda"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Lambda (props)](#apidoc.element.uglify-js.AST_Lambda.AST_Lambda)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>BASE (props)](#apidoc.element.uglify-js.AST_Lambda.BASE)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Lambda.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Lambda.SUBCLASSES"></a>[module uglify-js.AST_Lambda.SUBCLASSES](#apidoc.module.uglify-js.AST_Lambda.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Lambda.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Lambda.prototype"></a>[module uglify-js.AST_Lambda.prototype](#apidoc.module.uglify-js.AST_Lambda.prototype)

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Lambda.prototype.CTOR)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Lambda.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_do_print (output, nokeyword)](#apidoc.element.uglify-js.AST_Lambda.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, nokeyword){
    var self = this;
    if (!nokeyword) {
        output.print("function");
    }
    if (self.name) {
        output.space();
        self.name.print(output);
    }
    output.with_parens(function(){
        self.argnames.forEach(function(arg, i){
            if (i) output.comma();
            arg.print(output);
        });
    });
    output.space();
    print_bracketed(self.body, output, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Lambda.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Lambda.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        if (this.name) this.name._walk(visitor);
        var argnames = this.argnames;
        for (var i = 0, len = argnames.length; i < len; i++) {
            argnames[i]._walk(visitor);
        }
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Lambda.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype.init_scope_vars"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>init_scope_vars ()](#apidoc.element.uglify-js.AST_Lambda.prototype.init_scope_vars)
- description and source-code
```javascript
init_scope_vars = function (){
    AST_Scope.prototype.init_scope_vars.apply(this, arguments);
    this.uses_arguments = false;

    var symbol = new AST_VarDef({ name: "arguments", start: this.start, end: this.end });
    var def = new SymbolDef(this, this.variables.size(), symbol);
    this.variables.set(symbol.name, def);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Lambda.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Lambda.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Lambda.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Lambda.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_LoopControl"></a>[module uglify-js.AST_LoopControl](#apidoc.module.uglify-js.AST_LoopControl)

#### <a name="apidoc.element.uglify-js.AST_LoopControl.AST_LoopControl"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_LoopControl (props)](#apidoc.element.uglify-js.AST_LoopControl.AST_LoopControl)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LoopControl.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>BASE (props)](#apidoc.element.uglify-js.AST_LoopControl.BASE)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LoopControl.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_LoopControl.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_LoopControl.SUBCLASSES"></a>[module uglify-js.AST_LoopControl.SUBCLASSES](#apidoc.module.uglify-js.AST_LoopControl.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_LoopControl.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_LoopControl.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LoopControl.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_LoopControl.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_LoopControl.prototype"></a>[module uglify-js.AST_LoopControl.prototype](#apidoc.module.uglify-js.AST_LoopControl.prototype)

#### <a name="apidoc.element.uglify-js.AST_LoopControl.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_LoopControl.prototype.CTOR)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LoopControl.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>_do_print (output, kind)](#apidoc.element.uglify-js.AST_LoopControl.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, kind){
    output.print(kind);
    if (this.label) {
        output.space();
        this.label.print(output);
    }
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LoopControl.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_LoopControl.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, this.label && function(){
        this.label._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_LoopControl.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_LoopControl.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_LoopControl.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_NaN"></a>[module uglify-js.AST_NaN](#apidoc.module.uglify-js.AST_NaN)

#### <a name="apidoc.element.uglify-js.AST_NaN.AST_NaN"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_NaN (props)](#apidoc.element.uglify-js.AST_NaN.AST_NaN)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_NaN.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>BASE (props)](#apidoc.element.uglify-js.AST_NaN.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_NaN.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_NaN.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_NaN.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_NaN.prototype"></a>[module uglify-js.AST_NaN.prototype](#apidoc.module.uglify-js.AST_NaN.prototype)

#### <a name="apidoc.element.uglify-js.AST_NaN.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_NaN.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_NaN.prototype.CTOR)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_NaN.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_NaN.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_NaN.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("NaN");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_New"></a>[module uglify-js.AST_New](#apidoc.module.uglify-js.AST_New)

#### <a name="apidoc.element.uglify-js.AST_New.AST_New"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_New (props)](#apidoc.element.uglify-js.AST_New.AST_New)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.</span>BASE (props)](#apidoc.element.uglify-js.AST_New.BASE)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_New.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_New.prototype"></a>[module uglify-js.AST_New.prototype](#apidoc.module.uglify-js.AST_New.prototype)

#### <a name="apidoc.element.uglify-js.AST_New.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_New.prototype.CTOR)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_New.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("new");
    output.space();
    AST_Call.prototype._codegen(self, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_New.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_New.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    if (!need_constructor_parens(this, output)
        && (p instanceof AST_PropAccess // (new Date).getTime(), (new Date)["getTime"]()
            || p instanceof AST_Call && p.expression === this)) // (new foo)(bar)
        return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_New.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_New.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_New.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_New.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Node"></a>[module uglify-js.AST_Node](#apidoc.module.uglify-js.AST_Node)

#### <a name="apidoc.element.uglify-js.AST_Node.AST_Node"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Node (props)](#apidoc.element.uglify-js.AST_Node.AST_Node)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Node.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.from_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>from_mozilla_ast (node)](#apidoc.element.uglify-js.AST_Node.from_mozilla_ast)
- description and source-code
```javascript
from_mozilla_ast = function (node){
    var save_stack = FROM_MOZ_STACK;
    FROM_MOZ_STACK = [];
    var ast = from_moz(node);
    FROM_MOZ_STACK = save_stack;
    return ast;
}
```
- example usage
```shell
...
JavaScript ASTs in SpiderMonkey format.

Example:

'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = UglifyJS.Compressor(options).compress(uAST);

// Mangling (optional)
if (mangle) {
...
```

#### <a name="apidoc.element.uglify-js.AST_Node.warn"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>warn (txt, props)](#apidoc.element.uglify-js.AST_Node.warn)
- description and source-code
```javascript
warn = function (txt, props) {
    if (AST_Node.warn_function)
        AST_Node.warn_function(string_template(txt, props));
}
```
- example usage
```shell
...
}
else if (node instanceof AST_Sub) {
    if (!ignore_quoted)
        node.property = mangleStrings(node.property);
}
// else if (node instanceof AST_String) {
//     if (should_mangle(node.value)) {
//         AST_Node.warn(
//             "Found \"{prop}\" property candidate for mangling in an arbitrary string [{file}:{line},{col}]", {
//                 file : node.start.file,
//                 line : node.start.line,
//                 col  : node.start.col,
//                 prop : node.value
//             }
//         );
...
```

#### <a name="apidoc.element.uglify-js.AST_Node.warn_function"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.</span>warn_function (txt)](#apidoc.element.uglify-js.AST_Node.warn_function)
- description and source-code
```javascript
warn_function = function (txt) {
    console.error("WARN: %s", txt);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Node.SUBCLASSES"></a>[module uglify-js.AST_Node.SUBCLASSES](#apidoc.module.uglify-js.AST_Node.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.1)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.10"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>10 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.10)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.11"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>11 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.11)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.12"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>12 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.12)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.4)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.5)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.6"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>6 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.6)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.7"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>7 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.7)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.8"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>8 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.8)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.SUBCLASSES.9"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.SUBCLASSES.</span>9 (props)](#apidoc.element.uglify-js.AST_Node.SUBCLASSES.9)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Node.prototype"></a>[module uglify-js.AST_Node.prototype](#apidoc.module.uglify-js.AST_Node.prototype)

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Node.prototype.CTOR)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype._clone"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_clone (deep)](#apidoc.element.uglify-js.AST_Node.prototype._clone)
- description and source-code
```javascript
_clone = function (deep) {
    if (deep) {
        var self = this.clone();
        return self.transform(new TreeTransformer(function(node) {
            if (node !== self) {
                return node.clone(true);
            }
        }));
    }
    return new this.CTOR(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Node.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    throw def;          // not constant
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype._find_defs"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_find_defs ()](#apidoc.element.uglify-js.AST_Node.prototype._find_defs)
- description and source-code
```javascript
function noop() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Node.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.add_comments"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>add_comments (output)](#apidoc.element.uglify-js.AST_Node.prototype.add_comments)
- description and source-code
```javascript
add_comments = function (output){
    if (output._readonly) return;
    var self = this;
    var start = self.start;
    if (start && !start._comments_dumped) {
        start._comments_dumped = true;
        var comments = start.comments_before || [];

        // XXX: ugly fix for https://github.com/mishoo/UglifyJS2/issues/112
        //               and https://github.com/mishoo/UglifyJS2/issues/372
        if (self instanceof AST_Exit && self.value) {
            self.value.walk(new TreeWalker(function(node){
                if (node.start && node.start.comments_before) {
                    comments = comments.concat(node.start.comments_before);
                    node.start.comments_before = [];
                }
                if (node instanceof AST_Function ||
                    node instanceof AST_Array ||
                    node instanceof AST_Object)
                {
                    return true; // don't go inside.
                }
            }));
        }

        if (comments.length > 0 && output.pos() == 0) {
            if (output.option("shebang") && comments[0].type == "comment5") {
                output.print("#!" + comments.shift().value + "\n");
                output.indent();
            }
            var preamble = output.option("preamble");
            if (preamble) {
                output.print(preamble.replace(/\r\n?|[\n\u2028\u2029]|\s*$/g, "\n"));
            }
        }

        comments = comments.filter(output.comment_filter, self);

        // Keep single line comments after nlb, after nlb
        if (!output.option("beautify") && comments.length > 0 &&
            /comment[134]/.test(comments[0].type) &&
            output.col() !== 0 && comments[0].nlb)
        {
            output.print("\n");
        }

        comments.forEach(function(c){
            if (/comment[134]/.test(c.type)) {
                output.print("//" + c.value + "\n");
                output.indent();
            }
            else if (c.type == "comment2") {
                output.print("/*" + c.value + "*/");
                if (start.nlb) {
                    output.print("\n");
                    output.indent();
                } else {
                    output.space();
                }
            }
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Node.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.clone"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>clone (deep)](#apidoc.element.uglify-js.AST_Node.prototype.clone)
- description and source-code
```javascript
clone = function (deep) {
    return this._clone(deep);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.constant_value"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>constant_value (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.constant_value)
- description and source-code
```javascript
constant_value = function (compressor){
    // Accomodate when option evaluate=false.
    if (this instanceof AST_Constant && !(this instanceof AST_RegExp)) {
        return this.value;
    }
    // Accomodate the common constant expressions !0 and -1 when option evaluate=false.
    if (this instanceof AST_UnaryPrefix
        && this.expression instanceof AST_Constant) switch (this.operator) {
      case "!":
        return !this.expression.value;
      case "~":
        return ~this.expression.value;
      case "-":
        return -this.expression.value;
      case "+":
        return +this.expression.value;
      default:
        throw new Error(string_template("Cannot evaluate unary expression {value}", {
            value: this.print_to_string()
        }));
    }
    var result = this.evaluate(compressor);
    if (result !== this) {
        return result;
    }
    throw new Error(string_template("Cannot evaluate constant [{file}:{line},{col}]", this.start));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_Node.prototype.drop_side_effect_free)
- description and source-code
```javascript
function return_this() { return this; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.equivalent_to"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>equivalent_to (node)](#apidoc.element.uglify-js.AST_Node.prototype.equivalent_to)
- description and source-code
```javascript
equivalent_to = function (node){
    // XXX: this is a rather expensive way to test two node's equivalence:
    return this.print_to_string() == node.print_to_string();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>evaluate (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (compressor){
    if (!compressor.option("evaluate")) return this;
    try {
        var val = this._eval(compressor);
        return !val || val instanceof RegExp || typeof val != "object" ? val : this;
    } catch(ex) {
        if (ex !== def) throw ex;
        return this;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_Node.prototype.has_side_effects)
- description and source-code
```javascript
function return_true() { return true; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Node.prototype.is_boolean)
- description and source-code
```javascript
function return_false() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.is_constant"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_constant ()](#apidoc.element.uglify-js.AST_Node.prototype.is_constant)
- description and source-code
```javascript
is_constant = function (){
    // Accomodate when compress option evaluate=false
    // as well as the common constant expressions !0 and -1
    if (this instanceof AST_Constant) {
        return !(this instanceof AST_RegExp);
    } else {
        return this instanceof AST_UnaryPrefix
            && this.expression instanceof AST_Constant
            && unaryPrefix(this.operator);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.is_number"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_number ()](#apidoc.element.uglify-js.AST_Node.prototype.is_number)
- description and source-code
```javascript
function return_false() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>is_string ()](#apidoc.element.uglify-js.AST_Node.prototype.is_string)
- description and source-code
```javascript
function return_false() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>needs_parens ()](#apidoc.element.uglify-js.AST_Node.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (){
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Node.prototype.negate)
- description and source-code
```javascript
negate = function (compressor, first_in_statement){
    return func.call(this, compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.print"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>print (stream, force_parens)](#apidoc.element.uglify-js.AST_Node.prototype.print)
- description and source-code
```javascript
print = function (stream, force_parens){
    var self = this, generator = self._codegen, prev_use_asm = use_asm;
    if (self instanceof AST_Directive && self.value == "use asm" && stream.parent() instanceof AST_Scope) {
        use_asm = true;
    }
    function doit() {
        self.add_comments(stream);
        self.add_source_map(stream);
        generator(self, stream);
    }
    stream.push_node(self);
    if (force_parens || self.needs_parens(stream)) {
        stream.with_parens(doit);
    } else {
        doit();
    }
    stream.pop_node();
    if (self instanceof AST_Scope) {
        use_asm = prev_use_asm;
    }
}
```
- example usage
```shell
...

#### Generating output

AST nodes have a 'print' method that takes an output stream.  Essentially,
to generate code you do this:
'''javascript
var stream = UglifyJS.OutputStream(options);
compressed_ast.print(stream);
var code = stream.toString(); // this is your minified code
'''

or, for a shortcut you can do:
'''javascript
var code = compressed_ast.print_to_string(options);
'''
...
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.print_to_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>print_to_string (options)](#apidoc.element.uglify-js.AST_Node.prototype.print_to_string)
- description and source-code
```javascript
print_to_string = function (options){
    var s = OutputStream(options);
    if (!options) s._readonly = true;
    this.print(s);
    return s.get();
}
```
- example usage
```shell
...
var stream = UglifyJS.OutputStream(options);
compressed_ast.print(stream);
var code = stream.toString(); // this is your minified code
'''

or, for a shortcut you can do:
'''javascript
var code = compressed_ast.print_to_string(options);
'''

As usual, 'options' is optional.  The output stream accepts a lot of options,
most of them documented above in section “Beautifier options”.  The two
which we care about here are 'source_map' and 'comments'.

#### Keeping comments in the output
...
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.process_expression"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>process_expression (insert)](#apidoc.element.uglify-js.AST_Node.prototype.process_expression)
- description and source-code
```javascript
process_expression = function (insert) {
    var self = this;
    var tt = new TreeTransformer(function(node) {
        if (insert && node instanceof AST_SimpleStatement) {
            return make_node(AST_Return, node, {
                value: node.body
            });
        }
        if (!insert && node instanceof AST_Return) {
            return make_node(AST_SimpleStatement, node, {
                body: node.value || make_node(AST_Undefined, node)
            });
        }
        if (node instanceof AST_Lambda && node !== self) {
            return node;
        }
        if (node instanceof AST_Block) {
            var index = node.body.length - 1;
            if (index >= 0) {
                node.body[index] = node.body[index].transform(tt);
            }
        }
        if (node instanceof AST_If) {
            node.body = node.body.transform(tt);
            if (node.alternative) {
                node.alternative = node.alternative.transform(tt);
            }
        }
        if (node instanceof AST_With) {
            node.body = node.body.transform(tt);
        }
        return node;
    });
    return self.transform(tt);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.reset_opt_flags"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>reset_opt_flags (compressor, rescan)](#apidoc.element.uglify-js.AST_Node.prototype.reset_opt_flags)
- description and source-code
```javascript
reset_opt_flags = function (compressor, rescan){
    var reduce_vars = rescan && compressor.option("reduce_vars");
    var toplevel = compressor.option("toplevel");
    var ie8 = !compressor.option("screw_ie8");
    var safe_ids = [];
    push();
    var suppressor = new TreeWalker(function(node) {
        if (node instanceof AST_Symbol) {
            var d = node.definition();
            if (node instanceof AST_SymbolRef) d.references.push(node);
            d.fixed = false;
        }
    });
    var tw = new TreeWalker(function(node, descend){
        if (!(node instanceof AST_Directive || node instanceof AST_Constant)) {
            node._squeezed = false;
            node._optimized = false;
        }
        if (reduce_vars) {
            if (node instanceof AST_Toplevel) node.globals.each(reset_def);
            if (node instanceof AST_Scope) node.variables.each(reset_def);
            if (node instanceof AST_SymbolRef) {
                var d = node.definition();
                d.references.push(node);
                if (!d.fixed || !is_safe(d)
                    || is_modified(node, 0, d.fixed instanceof AST_Lambda)) {
                    d.fixed = false;
                }
            }
            if (ie8 && node instanceof AST_SymbolCatch) {
                node.definition().fixed = false;
            }
            if (node instanceof AST_VarDef) {
                var d = node.name.definition();
                if (d.fixed === undefined) {
                    d.fixed = node.value || make_node(AST_Undefined, node);
                    mark_as_safe(d);
                } else {
                    d.fixed = false;
                }
            }
            if (node instanceof AST_Defun) {
                var d = node.name.definition();
                if (!toplevel && d.global || is_safe(d)) {
                    d.fixed = false;
                } else {
                    d.fixed = node;
                    mark_as_safe(d);
                }
                var save_ids = safe_ids;
                safe_ids = [];
                push();
                descend();
                safe_ids = save_ids;
                return true;
            }
            var iife;
            if (node instanceof AST_Function
                && !node.name
                && (iife = tw.parent()) instanceof AST_Call
                && iife.expression === node) {
                // Virtually turn IIFE parameters into variable definitions:
                //   (function(a,b) {...})(c,d) => (function() {var a=c,b=d; ...})()
                // So existing transformation rules can work on them.
                node.argnames.forEach(function(arg, i) {
                    var d = arg.definition();
                    d.fixed = iife.args[i] || make_node(AST_Undefined, iife);
                    mark_as_safe(d);
                });
            }
            if (node instanceof AST_If || node instanceof AST_DWLoop) {
                node.condition.walk(tw);
                push();
                node.body.walk(tw);
                pop();
                if (node.alternative) {
                    push();
                    node.alternative.walk(tw);
                    pop();
                }
                return true;
            }
            if (node instanceof AST_LabeledStatement) {
                push();
                node.body.walk(tw);
                pop();
                return true;
            }
            if (node instanceof AST_For) {
                if (node.init) node.init.walk(tw);
                push();
                if (node.condition) node.condition.walk(tw);
                node.body.walk(tw);
                if (node.step) node.step.walk(tw);
                pop();
                return true;
            }
            if (node instanceof AST_ForIn) {
                node.init.walk(suppressor);
                node.object.walk(tw);
                push();
                node.body.walk(tw);
                pop();
                return true;
            }
            if (node instanceof AST_Catch) {
                push() ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.resolve_defines"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>resolve_defines (compressor)](#apidoc.element.uglify-js.AST_Node.prototype.resolve_defines)
- description and source-code
```javascript
resolve_defines = function (compressor) {
    if (!compressor.option("global_defs")) return;
    var def = this._find_defs(compressor, "");
    if (def) {
        var node, parent = this, level = 0;
        do {
            node = parent;
            parent = compressor.parent(level++);
        } while (parent instanceof AST_PropAccess && parent.expression === node);
        if (isLHS(node, parent)) {
            compressor.warn('global_defs ' + this.print_to_string() + ' redefined [{file}:{line},{col}]', this.start);
        } else {
            return def;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Node.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```

#### <a name="apidoc.element.uglify-js.AST_Node.prototype.walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Node.prototype.</span>walk (visitor)](#apidoc.element.uglify-js.AST_Node.prototype.walk)
- description and source-code
```javascript
walk = function (visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
```
- example usage
```shell
...
}

var names_to_mangle = [];
var unmangleable = [];
var ignored = {};

// step 1: find candidates to mangle
ast.walk(new TreeWalker(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        add(node.key, ignore_quoted && node.quote);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter, since KeyVal is handled above
        add(node.key.name);
    }
...
```



# <a name="apidoc.module.uglify-js.AST_Null"></a>[module uglify-js.AST_Null](#apidoc.module.uglify-js.AST_Null)

#### <a name="apidoc.element.uglify-js.AST_Null.AST_Null"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Null (props)](#apidoc.element.uglify-js.AST_Null.AST_Null)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Null.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>BASE (props)](#apidoc.element.uglify-js.AST_Null.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Null.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Null.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Null.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Null.prototype"></a>[module uglify-js.AST_Null.prototype](#apidoc.module.uglify-js.AST_Null.prototype)

#### <a name="apidoc.element.uglify-js.AST_Null.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Null.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Null.prototype.CTOR)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Null.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Null.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Null.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Number"></a>[module uglify-js.AST_Number](#apidoc.module.uglify-js.AST_Number)

#### <a name="apidoc.element.uglify-js.AST_Number.AST_Number"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Number (props)](#apidoc.element.uglify-js.AST_Number.AST_Number)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.literal = props.literal;this.value =
props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Number.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>BASE (props)](#apidoc.element.uglify-js.AST_Number.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Number.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Number.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Number.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Number.prototype"></a>[module uglify-js.AST_Number.prototype](#apidoc.module.uglify-js.AST_Number.prototype)

#### <a name="apidoc.element.uglify-js.AST_Number.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Number.prototype.CTOR)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.literal = props.literal;this.value =
props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Number.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Number.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    if (use_asm && self.start && self.start.raw != null) {
        output.print(self.start.raw);
    } else {
        output.print(make_num(self.getValue()));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Number.prototype.is_number"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>is_number ()](#apidoc.element.uglify-js.AST_Number.prototype.is_number)
- description and source-code
```javascript
function return_true() { return true; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Number.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Number.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Number.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    if (p instanceof AST_PropAccess && p.expression === this) {
        var value = this.getValue();
        if (value < 0 || /^0/.test(make_num(value))) {
            return true;
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Object"></a>[module uglify-js.AST_Object](#apidoc.module.uglify-js.AST_Object)

#### <a name="apidoc.element.uglify-js.AST_Object.AST_Object"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Object (props)](#apidoc.element.uglify-js.AST_Object.AST_Object)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>BASE (props)](#apidoc.element.uglify-js.AST_Object.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Object.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Object.prototype"></a>[module uglify-js.AST_Object.prototype](#apidoc.module.uglify-js.AST_Object.prototype)

#### <a name="apidoc.element.uglify-js.AST_Object.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Object.prototype.CTOR)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Object.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    if (self.properties.length > 0) output.with_block(function(){
        self.properties.forEach(function(prop, i){
            if (i) {
                output.print(",");
                output.newline();
            }
            output.indent();
            prop.print(output);
        });
        output.newline();
    });
    else output.print("{}");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_Object.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    if (compressor.option("unsafe")) {
        var val = {};
        for (var i = 0, len = this.properties.length; i < len; i++) {
            var prop = this.properties[i];
            var key = prop.key;
            if (key instanceof AST_Symbol) {
                key = key.name;
            } else if (key instanceof AST_Node) {
                key = ev(key, compressor);
            }
            if (typeof Object.prototype[key] === 'function') {
                throw def;
            }
            val[key] = ev(prop.value, compressor);
        }
        return val;
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Object.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        var properties = this.properties;
        for (var i = 0, len = properties.length; i < len; i++) {
            properties[i]._walk(visitor);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Object.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    var values = trim(this.properties, compressor, first_in_statement);
    return values && AST_Seq.from_array(values);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Object.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    for (var i = this.properties.length; --i >= 0;)
        if (this.properties[i].has_side_effects(compressor))
            return true;
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Object.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    return first_in_statement(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Object.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Object.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Object.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Object.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Object.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_ObjectGetter"></a>[module uglify-js.AST_ObjectGetter](#apidoc.module.uglify-js.AST_ObjectGetter)

#### <a name="apidoc.element.uglify-js.AST_ObjectGetter.AST_ObjectGetter"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectGetter (props)](#apidoc.element.uglify-js.AST_ObjectGetter.AST_ObjectGetter)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectGetter.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectGetter.BASE)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectGetter.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectGetter.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ObjectGetter.prototype"></a>[module uglify-js.AST_ObjectGetter.prototype](#apidoc.module.uglify-js.AST_ObjectGetter.prototype)

#### <a name="apidoc.element.uglify-js.AST_ObjectGetter.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectGetter.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectGetter.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ObjectGetter.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("get");
    output.space();
    self.key.print(output);
    self.value._do_print(output, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectGetter.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectGetter.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_ObjectGetter.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ObjectKeyVal"></a>[module uglify-js.AST_ObjectKeyVal](#apidoc.module.uglify-js.AST_ObjectKeyVal)

#### <a name="apidoc.element.uglify-js.AST_ObjectKeyVal.AST_ObjectKeyVal"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal.AST_ObjectKeyVal)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectKeyVal.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal.BASE)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectKeyVal.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectKeyVal.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ObjectKeyVal.prototype"></a>[module uglify-js.AST_ObjectKeyVal.prototype](#apidoc.module.uglify-js.AST_ObjectKeyVal.prototype)

#### <a name="apidoc.element.uglify-js.AST_ObjectKeyVal.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectKeyVal.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectKeyVal.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectKeyVal.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ObjectKeyVal.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var key = self.key;
    var quote = self.quote;
    if (output.option("quote_keys")) {
        output.print_string(key + "");
    } else if ((typeof key == "number"
                || !output.option("beautify")
                && +key + "" == key)
               && parseFloat(key) >= 0) {
        output.print(make_num(key));
    } else if (RESERVED_WORDS(key) ? output.option("screw_ie8") : is_identifier_string(key)) {
        if (quote && output.option("keep_quoted_props")) {
            output.print_string(key, quote);
        } else {
            output.print_name(key);
        }
    } else {
        output.print_string(key, quote);
    }
    output.colon();
    self.value.print(output);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ObjectProperty"></a>[module uglify-js.AST_ObjectProperty](#apidoc.module.uglify-js.AST_ObjectProperty)

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.AST_ObjectProperty"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectProperty (props)](#apidoc.element.uglify-js.AST_ObjectProperty.AST_ObjectProperty)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectProperty.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectProperty.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ObjectProperty.SUBCLASSES"></a>[module uglify-js.AST_ObjectProperty.SUBCLASSES](#apidoc.module.uglify-js.AST_ObjectProperty.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.0)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.1)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_ObjectProperty.SUBCLASSES.2)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ObjectProperty.prototype"></a>[module uglify-js.AST_ObjectProperty.prototype](#apidoc.module.uglify-js.AST_ObjectProperty.prototype)

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.value._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    return this.value.drop_side_effect_free(compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.value.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_ObjectProperty.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectProperty.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_ObjectProperty.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_ObjectSetter"></a>[module uglify-js.AST_ObjectSetter](#apidoc.module.uglify-js.AST_ObjectSetter)

#### <a name="apidoc.element.uglify-js.AST_ObjectSetter.AST_ObjectSetter"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_ObjectSetter (props)](#apidoc.element.uglify-js.AST_ObjectSetter.AST_ObjectSetter)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectSetter.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>BASE (props)](#apidoc.element.uglify-js.AST_ObjectSetter.BASE)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectSetter.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_ObjectSetter.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_ObjectSetter.prototype"></a>[module uglify-js.AST_ObjectSetter.prototype](#apidoc.module.uglify-js.AST_ObjectSetter.prototype)

#### <a name="apidoc.element.uglify-js.AST_ObjectSetter.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_ObjectSetter.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectSetter.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_ObjectSetter.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("set");
    output.space();
    self.key.print(output);
    self.value._do_print(output, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_ObjectSetter.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_ObjectSetter.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_ObjectSetter.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_PropAccess"></a>[module uglify-js.AST_PropAccess](#apidoc.module.uglify-js.AST_PropAccess)

#### <a name="apidoc.element.uglify-js.AST_PropAccess.AST_PropAccess"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_PropAccess (props)](#apidoc.element.uglify-js.AST_PropAccess.AST_PropAccess)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>BASE (props)](#apidoc.element.uglify-js.AST_PropAccess.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_PropAccess.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_PropAccess.SUBCLASSES"></a>[module uglify-js.AST_PropAccess.SUBCLASSES](#apidoc.module.uglify-js.AST_PropAccess.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_PropAccess.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_PropAccess.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_PropAccess.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_PropAccess.prototype"></a>[module uglify-js.AST_PropAccess.prototype](#apidoc.module.uglify-js.AST_PropAccess.prototype)

#### <a name="apidoc.element.uglify-js.AST_PropAccess.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_PropAccess.prototype.CTOR)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_PropAccess.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    if (compressor.option("unsafe")) {
        var key = this.property;
        if (key instanceof AST_Node) {
            key = ev(key, compressor);
        }
        var val = ev(this.expression, compressor);
        if (val && HOP(val, key)) {
            return val[key];
        }
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_PropAccess.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return !compressor.option("pure_getters");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_PropAccess.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    if (p instanceof AST_New && p.expression === this) {
        // i.e. new (foo.bar().baz)
        //
        // if there's one call into this subtree, then we need
        // parens around it too, otherwise the call will be
        // interpreted as passing the arguments to the upper New
        // expression.
        try {
            this.walk(new TreeWalker(function(node){
                if (node instanceof AST_Call) throw p;
            }));
        } catch(ex) {
            if (ex !== p) throw ex;
            return true;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_PropAccess.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_PropAccess.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_PropAccess.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_RegExp"></a>[module uglify-js.AST_RegExp](#apidoc.module.uglify-js.AST_RegExp)

#### <a name="apidoc.element.uglify-js.AST_RegExp.AST_RegExp"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_RegExp (props)](#apidoc.element.uglify-js.AST_RegExp.AST_RegExp)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_RegExp.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>BASE (props)](#apidoc.element.uglify-js.AST_RegExp.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_RegExp.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_RegExp.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_RegExp.prototype"></a>[module uglify-js.AST_RegExp.prototype](#apidoc.module.uglify-js.AST_RegExp.prototype)

#### <a name="apidoc.element.uglify-js.AST_RegExp.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_RegExp.prototype.CTOR)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_RegExp.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_RegExp.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var str = self.getValue().toString();
    if (output.option("ascii_only")) {
        str = output.to_ascii(str);
    } else if (output.option("unescape_regexps")) {
        str = str.split("\\\\").map(function(str){
            return str.replace(/\\u[0-9a-fA-F]{4}|\\x[0-9a-fA-F]{2}/g, function(s){
                var code = parseInt(s.substr(2), 16);
                return regexp_safe_literal(code) ? String.fromCharCode(code) : s;
            });
        }).join("\\\\");
    }
    output.print(str);
    var p = output.parent();
    if (p instanceof AST_Binary && /^in/.test(p.operator) && p.left === self)
        output.print(" ");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_RegExp.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_RegExp.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_RegExp.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_RegExp.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_RegExp.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Return"></a>[module uglify-js.AST_Return](#apidoc.module.uglify-js.AST_Return)

#### <a name="apidoc.element.uglify-js.AST_Return.AST_Return"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Return (props)](#apidoc.element.uglify-js.AST_Return.AST_Return)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Return.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>BASE (props)](#apidoc.element.uglify-js.AST_Return.BASE)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Return.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Return.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Return.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Return.prototype"></a>[module uglify-js.AST_Return.prototype](#apidoc.module.uglify-js.AST_Return.prototype)

#### <a name="apidoc.element.uglify-js.AST_Return.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Return.prototype.CTOR)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Return.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Return.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "return");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Return.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Return.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Return.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Return.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Return.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Scope"></a>[module uglify-js.AST_Scope](#apidoc.module.uglify-js.AST_Scope)

#### <a name="apidoc.element.uglify-js.AST_Scope.AST_Scope"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Scope (props)](#apidoc.element.uglify-js.AST_Scope.AST_Scope)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>BASE (props)](#apidoc.element.uglify-js.AST_Scope.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Scope.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Scope.SUBCLASSES"></a>[module uglify-js.AST_Scope.SUBCLASSES](#apidoc.module.uglify-js.AST_Scope.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Scope.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Scope.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Scope.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Scope.prototype"></a>[module uglify-js.AST_Scope.prototype](#apidoc.module.uglify-js.AST_Scope.prototype)

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Scope.prototype.CTOR)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.def_function"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>def_function (symbol)](#apidoc.element.uglify-js.AST_Scope.prototype.def_function)
- description and source-code
```javascript
def_function = function (symbol){
    this.functions.set(symbol.name, this.def_variable(symbol));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.def_variable"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>def_variable (symbol)](#apidoc.element.uglify-js.AST_Scope.prototype.def_variable)
- description and source-code
```javascript
def_variable = function (symbol){
    var def;
    if (!this.variables.has(symbol.name)) {
        def = new SymbolDef(this, this.variables.size(), symbol);
        this.variables.set(symbol.name, def);
        def.global = !this.parent_scope;
    } else {
        def = this.variables.get(symbol.name);
        def.orig.push(symbol);
    }
    return symbol.thedef = def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.drop_unused"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>drop_unused (compressor)](#apidoc.element.uglify-js.AST_Scope.prototype.drop_unused)
- description and source-code
```javascript
drop_unused = function (compressor){
    var self = this;
    if (compressor.has_directive("use asm")) return self;
    var toplevel = compressor.option("toplevel");
    if (compressor.option("unused")
        && (!(self instanceof AST_Toplevel) || toplevel)
        && !self.uses_eval
        && !self.uses_with) {
        var assign_as_unused = !/keep_assign/.test(compressor.option("unused"));
        var drop_funcs = /funcs/.test(toplevel);
        var drop_vars = /vars/.test(toplevel);
        if (!(self instanceof AST_Toplevel) || toplevel == true) {
            drop_funcs = drop_vars = true;
        }
        var in_use = [];
        var in_use_ids = Object.create(null); // avoid expensive linear scans of in_use
        if (self instanceof AST_Toplevel && compressor.top_retain) {
            self.variables.each(function(def) {
                if (compressor.top_retain(def) && !(def.id in in_use_ids)) {
                    in_use_ids[def.id] = true;
                    in_use.push(def);
                }
            });
        }
        var initializations = new Dictionary();
        // pass 1: find out which symbols are directly used in
        // this scope (not in nested scopes).
        var scope = this;
        var tw = new TreeWalker(function(node, descend){
            if (node !== self) {
                if (node instanceof AST_Defun) {
                    if (!drop_funcs && scope === self) {
                        var node_def = node.name.definition();
                        if (!(node_def.id in in_use_ids)) {
                            in_use_ids[node_def.id] = true;
                            in_use.push(node_def);
                        }
                    }
                    initializations.add(node.name.name, node);
                    return true; // don't go in nested scopes
                }
                if (node instanceof AST_Definitions && scope === self) {
                    node.definitions.forEach(function(def){
                        if (!drop_vars) {
                            var node_def = def.name.definition();
                            if (!(node_def.id in in_use_ids)) {
                                in_use_ids[node_def.id] = true;
                                in_use.push(node_def);
                            }
                        }
                        if (def.value) {
                            initializations.add(def.name.name, def.value);
                            if (def.value.has_side_effects(compressor)) {
                                def.value.walk(tw);
                            }
                        }
                    });
                    return true;
                }
                if (assign_as_unused
                    && node instanceof AST_Assign
                    && node.operator == "="
                    && node.left instanceof AST_SymbolRef
                    && scope === self) {
                    node.right.walk(tw);
                    return true;
                }
                if (node instanceof AST_SymbolRef) {
                    var node_def = node.definition();
                    if (!(node_def.id in in_use_ids)) {
                        in_use_ids[node_def.id] = true;
                        in_use.push(node_def);
                    }
                    return true;
                }
                if (node instanceof AST_Scope) {
                    var save_scope = scope;
                    scope = node;
                    descend();
                    scope = save_scope;
                    return true;
                }
            }
        });
        self.walk(tw);
        // pass 2: for every used symbol we need to walk its
        // initialization code to figure out if it uses other
        // symbols (that may not be in_use).
        for (var i = 0; i < in_use.length; ++i) {
            in_use[i].orig.forEach(function(decl){
                // undeclared globals will be instanceof AST_SymbolRef
                var init = initializations.get(decl.name);
                if (init) init.forEach(functio ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.find_variable"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>find_variable (name)](#apidoc.element.uglify-js.AST_Scope.prototype.find_variable)
- description and source-code
```javascript
find_variable = function (name){
    if (name instanceof AST_Symbol) name = name.name;
    return this.variables.get(name)
        || (this.parent_scope && this.parent_scope.find_variable(name));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.hoist_declarations"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>hoist_declarations (compressor)](#apidoc.element.uglify-js.AST_Scope.prototype.hoist_declarations)
- description and source-code
```javascript
hoist_declarations = function (compressor){
    var self = this;
    if (compressor.has_directive("use asm")) return self;
    var hoist_funs = compressor.option("hoist_funs");
    var hoist_vars = compressor.option("hoist_vars");
    if (hoist_funs || hoist_vars) {
        var dirs = [];
        var hoisted = [];
        var vars = new Dictionary(), vars_found = 0, var_decl = 0;
        // let's count var_decl first, we seem to waste a lot of
        // space if we hoist 'var' when there's only one.
        self.walk(new TreeWalker(function(node){
            if (node instanceof AST_Scope && node !== self)
                return true;
            if (node instanceof AST_Var) {
                ++var_decl;
                return true;
            }
        }));
        hoist_vars = hoist_vars && var_decl > 1;
        var tt = new TreeTransformer(
            function before(node) {
                if (node !== self) {
                    if (node instanceof AST_Directive) {
                        dirs.push(node);
                        return make_node(AST_EmptyStatement, node);
                    }
                    if (node instanceof AST_Defun && hoist_funs) {
                        hoisted.push(node);
                        return make_node(AST_EmptyStatement, node);
                    }
                    if (node instanceof AST_Var && hoist_vars) {
                        node.definitions.forEach(function(def){
                            vars.set(def.name.name, def);
                            ++vars_found;
                        });
                        var seq = node.to_assignments(compressor);
                        var p = tt.parent();
                        if (p instanceof AST_ForIn && p.init === node) {
                            if (seq == null) {
                                var def = node.definitions[0].name;
                                return make_node(AST_SymbolRef, def, def);
                            }
                            return seq;
                        }
                        if (p instanceof AST_For && p.init === node) {
                            return seq;
                        }
                        if (!seq) return make_node(AST_EmptyStatement, node);
                        return make_node(AST_SimpleStatement, node, {
                            body: seq
                        });
                    }
                    if (node instanceof AST_Scope)
                        return node; // to avoid descending in nested scopes
                }
            }
        );
        self = self.transform(tt);
        if (vars_found > 0) {
            // collect only vars which don't show up in self's arguments list
            var defs = [];
            vars.each(function(def, name){
                if (self instanceof AST_Lambda
                    && find_if(function(x){ return x.name == def.name.name },
                               self.argnames)) {
                    vars.del(name);
                } else {
                    def = def.clone();
                    def.value = null;
                    defs.push(def);
                    vars.set(name, def);
                }
            });
            if (defs.length > 0) {
                // try to merge in assignments
                for (var i = 0; i < self.body.length;) {
                    if (self.body[i] instanceof AST_SimpleStatement) {
                        var expr = self.body[i].body, sym, assign;
                        if (expr instanceof AST_Assign
                            && expr.operator == "="
                            && (sym = expr.left) instanceof AST_Symbol
                            && vars.has(sym.name))
                        {
                            var def = vars.get(sym.name);
                            if (def.value) break;
                            def.value = expr.right;
                            remove(defs, def);
                            defs.push(def);
                            self.body.splice(i, 1);
                            continue; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.init_scope_vars"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>init_scope_vars ()](#apidoc.element.uglify-js.AST_Scope.prototype.init_scope_vars)
- description and source-code
```javascript
init_scope_vars = function (){
    this.variables = new Dictionary(); // map name to AST_SymbolVar (variables defined in this scope; includes functions)
    this.functions = new Dictionary(); // map name to AST_SymbolDefun (functions defined in this scope)
    this.uses_with = false;   // will be set to true if this or some nested scope uses the 'with' statement
    this.uses_eval = false;   // will be set to true if this or nested scope uses the global 'eval'
    this.parent_scope = null; // the parent scope
    this.enclosed = [];       // a list of variables from this or outer scope(s) that are referenced from this or inner scopes
    this.cname = -1;          // the current index for mangling functions/variables
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Scope.prototype.next_mangled"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Scope.prototype.</span>next_mangled (options)](#apidoc.element.uglify-js.AST_Scope.prototype.next_mangled)
- description and source-code
```javascript
next_mangled = function (options){
    var ext = this.enclosed;
    out: while (true) {
        var m = base54(++this.cname);
        if (!is_identifier(m)) continue; // skip over "do"

        // https://github.com/mishoo/UglifyJS2/issues/242 -- do not
        // shadow a name excepted from mangling.
        if (options.except.indexOf(m) >= 0) continue;

        // we must ensure that the mangled name does not shadow a name
        // from some parent scope that is referenced in this or in
        // inner scopes.
        for (var i = ext.length; --i >= 0;) {
            var sym = ext[i];
            var name = sym.mangled_name || (sym.unmangleable(options) && sym.name);
            if (m == name) continue out;
        }
        return m;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Seq"></a>[module uglify-js.AST_Seq](#apidoc.module.uglify-js.AST_Seq)

#### <a name="apidoc.element.uglify-js.AST_Seq.AST_Seq"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Seq (props)](#apidoc.element.uglify-js.AST_Seq.AST_Seq)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>BASE (props)](#apidoc.element.uglify-js.AST_Seq.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Seq.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.cons"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>cons (x, y)](#apidoc.element.uglify-js.AST_Seq.cons)
- description and source-code
```javascript
cons = function (x, y) {
    var seq = new AST_Seq(x);
    seq.car = x;
    seq.cdr = y;
    return seq;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.from_array"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.</span>from_array (array)](#apidoc.element.uglify-js.AST_Seq.from_array)
- description and source-code
```javascript
from_array = function (array) {
    if (array.length == 0) return null;
    if (array.length == 1) return array[0].clone();
    var list = null;
    for (var i = array.length; --i >= 0;) {
        list = AST_Seq.cons(array[i], list);
    }
    var p = list;
    while (p) {
        if (p.cdr && !p.cdr.cdr) {
            p.cdr = p.cdr.car;
            break;
        }
        p = p.cdr;
    }
    return list;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Seq.prototype"></a>[module uglify-js.AST_Seq.prototype](#apidoc.module.uglify-js.AST_Seq.prototype)

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Seq.prototype.CTOR)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Seq.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output);
    // var p = output.parent();
    // if (p instanceof AST_Statement) {
    //     output.with_indent(output.next_indent(), function(){
    //         self._do_print(output);
    //     });
    // } else {
    //     self._do_print(output);
    // }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>_do_print (output)](#apidoc.element.uglify-js.AST_Seq.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output){
    this.car.print(output);
    if (this.cdr) {
        output.comma();
        if (output.should_break()) {
            output.newline();
            output.indent();
        }
        this.cdr.print(output);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Seq.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.car._walk(visitor);
        if (this.cdr) this.cdr._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.add"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>add (node)](#apidoc.element.uglify-js.AST_Seq.prototype.add)
- description and source-code
```javascript
add = function (node) {
    var p = this;
    while (p) {
        if (!(p.cdr instanceof AST_Seq)) {
            var cell = AST_Seq.cons(p.cdr, node);
            return p.cdr = cell;
        }
        p = p.cdr;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>drop_side_effect_free (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor){
    var cdr = this.cdr.drop_side_effect_free(compressor);
    if (cdr === this.cdr) return this;
    if (!cdr) return this.car;
    return make_node(AST_Seq, this, {
        car: this.car,
        cdr: cdr
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.car.has_side_effects(compressor)
        || this.cdr.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_Seq.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return this.cdr.is_boolean();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.is_number"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>is_number (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.is_number)
- description and source-code
```javascript
is_number = function (compressor){
    return this.cdr.is_number(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>is_string (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return this.cdr.is_string(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.len"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>len ()](#apidoc.element.uglify-js.AST_Seq.prototype.len)
- description and source-code
```javascript
len = function () {
    if (this.cdr instanceof AST_Seq) {
        return this.cdr.len() + 1;
    } else {
        return 2;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Seq.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    return p instanceof AST_Call             // (foo, bar)() or foo(1, (2, 3), 4)
        || p instanceof AST_Unary            // !(foo, bar, baz)
        || p instanceof AST_Binary           // 1 + (2, 3) + 4 ==> 8
        || p instanceof AST_VarDef           // var a = (1, 2), b = a + a; ==> b == 4
        || p instanceof AST_PropAccess       // (1, {foo:2}).foo or (1, {foo:2})["foo"] ==> 2
        || p instanceof AST_Array            // [ 1, (2, 3), 4 ] ==> [ 1, 3, 4 ]
        || p instanceof AST_ObjectProperty   // { foo: (1, 2) }.foo ==> 2
        || p instanceof AST_Conditional<span class="apidocCodeCommentSpan">      /* (false, true) ? (a = 10, b = 20) : (c = 30)
                                              * ==> 20 (side effect, set a := 10 and b := 20) */
</span>    ;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Seq.prototype.negate)
- description and source-code
```javascript
negate = function (compressor, first_in_statement){
    return func.call(this, compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Seq.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.to_array"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>to_array ()](#apidoc.element.uglify-js.AST_Seq.prototype.to_array)
- description and source-code
```javascript
to_array = function () {
    var p = this, a = [];
    while (p) {
        a.push(p.car);
        if (p.cdr && !(p.cdr instanceof AST_Seq)) {
            a.push(p.cdr);
            break;
        }
        p = p.cdr;
    }
    return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Seq.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Seq.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Seq.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Seq.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_SimpleStatement"></a>[module uglify-js.AST_SimpleStatement](#apidoc.module.uglify-js.AST_SimpleStatement)

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.AST_SimpleStatement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SimpleStatement (props)](#apidoc.element.uglify-js.AST_SimpleStatement.AST_SimpleStatement)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>BASE (props)](#apidoc.element.uglify-js.AST_SimpleStatement.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SimpleStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SimpleStatement.prototype"></a>[module uglify-js.AST_SimpleStatement.prototype](#apidoc.module.uglify-js.AST_SimpleStatement.prototype)

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.body.print(output);
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.body.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_SimpleStatement.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SimpleStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_SimpleStatement.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Statement"></a>[module uglify-js.AST_Statement](#apidoc.module.uglify-js.AST_Statement)

#### <a name="apidoc.element.uglify-js.AST_Statement.AST_Statement"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Statement (props)](#apidoc.element.uglify-js.AST_Statement.AST_Statement)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>BASE (props)](#apidoc.element.uglify-js.AST_Statement.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Statement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Statement.SUBCLASSES"></a>[module uglify-js.AST_Statement.SUBCLASSES](#apidoc.module.uglify-js.AST_Statement.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.2)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.4)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.5)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.6"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>6 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.6)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.SUBCLASSES.7"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.SUBCLASSES.</span>7 (props)](#apidoc.element.uglify-js.AST_Statement.SUBCLASSES.7)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Statement.prototype"></a>[module uglify-js.AST_Statement.prototype](#apidoc.module.uglify-js.AST_Statement.prototype)

#### <a name="apidoc.element.uglify-js.AST_Statement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Statement.prototype.CTOR)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Statement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.body.print(output);
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>_eval ()](#apidoc.element.uglify-js.AST_Statement.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    throw new Error(string_template("Cannot evaluate a statement [{file}:{line},{col}]", this.start));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_Statement.prototype.aborts)
- description and source-code
```javascript
function return_null() { return null; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Statement.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Statement.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Statement.prototype.negate)
- description and source-code
```javascript
negate = function (compressor, first_in_statement){
    return func.call(this, compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_StatementWithBody"></a>[module uglify-js.AST_StatementWithBody](#apidoc.module.uglify-js.AST_StatementWithBody)

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.AST_StatementWithBody"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_StatementWithBody (props)](#apidoc.element.uglify-js.AST_StatementWithBody.AST_StatementWithBody)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>BASE (props)](#apidoc.element.uglify-js.AST_StatementWithBody.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_StatementWithBody.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_StatementWithBody.SUBCLASSES"></a>[module uglify-js.AST_StatementWithBody.SUBCLASSES](#apidoc.module.uglify-js.AST_StatementWithBody.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.0)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.1)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.2)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_StatementWithBody.SUBCLASSES.3)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_StatementWithBody.prototype"></a>[module uglify-js.AST_StatementWithBody.prototype](#apidoc.module.uglify-js.AST_StatementWithBody.prototype)

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype.CTOR)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.prototype._do_print_body"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>_do_print_body (output)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype._do_print_body)
- description and source-code
```javascript
_do_print_body = function (output){
    force_statement(this.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_StatementWithBody.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_StatementWithBody.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_StatementWithBody.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_String"></a>[module uglify-js.AST_String](#apidoc.module.uglify-js.AST_String)

#### <a name="apidoc.element.uglify-js.AST_String.AST_String"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_String (props)](#apidoc.element.uglify-js.AST_String.AST_String)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_String.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_String.</span>BASE (props)](#apidoc.element.uglify-js.AST_String.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_String.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_String.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_String.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_String.prototype"></a>[module uglify-js.AST_String.prototype](#apidoc.module.uglify-js.AST_String.prototype)

#### <a name="apidoc.element.uglify-js.AST_String.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_String.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_String.prototype.CTOR)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_String.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_String.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_String.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print_string(self.getValue(), self.quote, in_directive);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_String.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_String.prototype.</span>is_string ()](#apidoc.element.uglify-js.AST_String.prototype.is_string)
- description and source-code
```javascript
function return_true() { return true; }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Sub"></a>[module uglify-js.AST_Sub](#apidoc.module.uglify-js.AST_Sub)

#### <a name="apidoc.element.uglify-js.AST_Sub.AST_Sub"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Sub (props)](#apidoc.element.uglify-js.AST_Sub.AST_Sub)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>BASE (props)](#apidoc.element.uglify-js.AST_Sub.BASE)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Sub.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Sub.prototype"></a>[module uglify-js.AST_Sub.prototype](#apidoc.module.uglify-js.AST_Sub.prototype)

#### <a name="apidoc.element.uglify-js.AST_Sub.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Sub.prototype.CTOR)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Sub.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.expression.print(output);
    output.print("[");
    self.property.print(output);
    output.print("]");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Sub.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        this.property._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Sub.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    if (!compressor.option("pure_getters")) return this;
    var expression = this.expression.drop_side_effect_free(compressor, first_in_statement);
    if (!expression) return this.property.drop_side_effect_free(compressor, first_in_statement);
    var property = this.property.drop_side_effect_free(compressor);
    if (!property) return expression;
    return make_node(AST_Seq, this, {
        car: expression,
        cdr: property
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Sub.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    if (!compressor.option("pure_getters")) return true;
    return this.expression.has_side_effects(compressor)
        || this.property.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Sub.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Sub.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Sub.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Sub.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Switch"></a>[module uglify-js.AST_Switch](#apidoc.module.uglify-js.AST_Switch)

#### <a name="apidoc.element.uglify-js.AST_Switch.AST_Switch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Switch (props)](#apidoc.element.uglify-js.AST_Switch.AST_Switch)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>BASE (props)](#apidoc.element.uglify-js.AST_Switch.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Switch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Switch.prototype"></a>[module uglify-js.AST_Switch.prototype](#apidoc.module.uglify-js.AST_Switch.prototype)

#### <a name="apidoc.element.uglify-js.AST_Switch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Switch.prototype.CTOR)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Switch.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("switch");
    output.space();
    output.with_parens(function(){
        self.expression.print(output);
    });
    output.space();
    if (self.body.length > 0) output.with_block(function(){
        self.body.forEach(function(stmt, i){
            if (i) output.newline();
            output.indent(true);
            stmt.print(output);
        });
    });
    else output.print("{}");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Switch.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Switch.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Switch.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Switch.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Switch.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Switch.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Switch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Switch.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_SwitchBranch"></a>[module uglify-js.AST_SwitchBranch](#apidoc.module.uglify-js.AST_SwitchBranch)

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.AST_SwitchBranch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SwitchBranch (props)](#apidoc.element.uglify-js.AST_SwitchBranch.AST_SwitchBranch)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>BASE (props)](#apidoc.element.uglify-js.AST_SwitchBranch.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SwitchBranch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SwitchBranch.SUBCLASSES"></a>[module uglify-js.AST_SwitchBranch.SUBCLASSES](#apidoc.module.uglify-js.AST_SwitchBranch.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_SwitchBranch.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_SwitchBranch.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SwitchBranch.prototype"></a>[module uglify-js.AST_SwitchBranch.prototype](#apidoc.module.uglify-js.AST_SwitchBranch.prototype)

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.CTOR)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.prototype._do_print_body"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>_do_print_body (output)](#apidoc.element.uglify-js.AST_SwitchBranch.prototype._do_print_body)
- description and source-code
```javascript
_do_print_body = function (output){
    if (this.body.length > 0) {
        output.newline();
        this.body.forEach(function(stmt){
            output.indent();
            stmt.print(output);
            output.newline();
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>aborts ()](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.aborts)
- description and source-code
```javascript
function block_aborts(){
    var n = this.body.length;
    return n > 0 && aborts(this.body[n - 1]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SwitchBranch.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SwitchBranch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_SwitchBranch.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Symbol"></a>[module uglify-js.AST_Symbol](#apidoc.module.uglify-js.AST_Symbol)

#### <a name="apidoc.element.uglify-js.AST_Symbol.AST_Symbol"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Symbol (props)](#apidoc.element.uglify-js.AST_Symbol.AST_Symbol)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>BASE (props)](#apidoc.element.uglify-js.AST_Symbol.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Symbol.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Symbol.SUBCLASSES"></a>[module uglify-js.AST_Symbol.SUBCLASSES](#apidoc.module.uglify-js.AST_Symbol.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.0)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.1)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.3)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.4)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.SUBCLASSES.</span>5 (props)](#apidoc.element.uglify-js.AST_Symbol.SUBCLASSES.5)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Symbol.prototype"></a>[module uglify-js.AST_Symbol.prototype](#apidoc.module.uglify-js.AST_Symbol.prototype)

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Symbol.prototype.CTOR)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Symbol.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var def = self.definition();
    output.print_name(def ? def.mangled_name || def.name : self.name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Symbol.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.definition"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>definition ()](#apidoc.element.uglify-js.AST_Symbol.prototype.definition)
- description and source-code
```javascript
definition = function (){
    return this.thedef;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.global"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>global ()](#apidoc.element.uglify-js.AST_Symbol.prototype.global)
- description and source-code
```javascript
global = function (){
    return this.definition().global;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Symbol.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.undeclared"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>undeclared ()](#apidoc.element.uglify-js.AST_Symbol.prototype.undeclared)
- description and source-code
```javascript
undeclared = function (){
    return this.definition().undeclared;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>unmangleable (options)](#apidoc.element.uglify-js.AST_Symbol.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (options){
    return this.definition().unmangleable(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Symbol.prototype.unreferenced"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Symbol.prototype.</span>unreferenced ()](#apidoc.element.uglify-js.AST_Symbol.prototype.unreferenced)
- description and source-code
```javascript
unreferenced = function (){
    return this.definition().references.length == 0
        && !(this.scope.uses_eval || this.scope.uses_with);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolAccessor"></a>[module uglify-js.AST_SymbolAccessor](#apidoc.module.uglify-js.AST_SymbolAccessor)

#### <a name="apidoc.element.uglify-js.AST_SymbolAccessor.AST_SymbolAccessor"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolAccessor (props)](#apidoc.element.uglify-js.AST_SymbolAccessor.AST_SymbolAccessor)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolAccessor.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolAccessor.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolAccessor.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolAccessor.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolAccessor.prototype"></a>[module uglify-js.AST_SymbolAccessor.prototype](#apidoc.module.uglify-js.AST_SymbolAccessor.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolAccessor.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolAccessor.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolAccessor.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolAccessor.prototype.</span>unmangleable ()](#apidoc.element.uglify-js.AST_SymbolAccessor.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (){
    return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolCatch"></a>[module uglify-js.AST_SymbolCatch](#apidoc.module.uglify-js.AST_SymbolCatch)

#### <a name="apidoc.element.uglify-js.AST_SymbolCatch.AST_SymbolCatch"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolCatch (props)](#apidoc.element.uglify-js.AST_SymbolCatch.AST_SymbolCatch)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolCatch.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolCatch.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolCatch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolCatch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolCatch.prototype"></a>[module uglify-js.AST_SymbolCatch.prototype](#apidoc.module.uglify-js.AST_SymbolCatch.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolCatch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolCatch.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolCatch.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolConst"></a>[module uglify-js.AST_SymbolConst](#apidoc.module.uglify-js.AST_SymbolConst)

#### <a name="apidoc.element.uglify-js.AST_SymbolConst.AST_SymbolConst"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolConst (props)](#apidoc.element.uglify-js.AST_SymbolConst.AST_SymbolConst)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolConst.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolConst.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolConst.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolConst.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolConst.prototype"></a>[module uglify-js.AST_SymbolConst.prototype](#apidoc.module.uglify-js.AST_SymbolConst.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolConst.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolConst.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolConst.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolDeclaration"></a>[module uglify-js.AST_SymbolDeclaration](#apidoc.module.uglify-js.AST_SymbolDeclaration)

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.AST_SymbolDeclaration"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.AST_SymbolDeclaration)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolDeclaration.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolDeclaration.SUBCLASSES"></a>[module uglify-js.AST_SymbolDeclaration.SUBCLASSES](#apidoc.module.uglify-js.AST_SymbolDeclaration.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.0)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.1)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>2 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.2)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>3 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.3)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.SUBCLASSES.</span>4 (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.SUBCLASSES.4)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolDeclaration.prototype"></a>[module uglify-js.AST_SymbolDeclaration.prototype](#apidoc.module.uglify-js.AST_SymbolDeclaration.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolDeclaration.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDeclaration.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolDeclaration.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolDefun"></a>[module uglify-js.AST_SymbolDefun](#apidoc.module.uglify-js.AST_SymbolDefun)

#### <a name="apidoc.element.uglify-js.AST_SymbolDefun.AST_SymbolDefun"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolDefun (props)](#apidoc.element.uglify-js.AST_SymbolDefun.AST_SymbolDefun)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDefun.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolDefun.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolDefun.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolDefun.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolDefun.prototype"></a>[module uglify-js.AST_SymbolDefun.prototype](#apidoc.module.uglify-js.AST_SymbolDefun.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolDefun.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolDefun.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolDefun.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolFunarg"></a>[module uglify-js.AST_SymbolFunarg](#apidoc.module.uglify-js.AST_SymbolFunarg)

#### <a name="apidoc.element.uglify-js.AST_SymbolFunarg.AST_SymbolFunarg"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolFunarg (props)](#apidoc.element.uglify-js.AST_SymbolFunarg.AST_SymbolFunarg)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolFunarg.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolFunarg.BASE)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolFunarg.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolFunarg.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolFunarg.prototype"></a>[module uglify-js.AST_SymbolFunarg.prototype](#apidoc.module.uglify-js.AST_SymbolFunarg.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolFunarg.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolFunarg.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolFunarg.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolLambda"></a>[module uglify-js.AST_SymbolLambda](#apidoc.module.uglify-js.AST_SymbolLambda)

#### <a name="apidoc.element.uglify-js.AST_SymbolLambda.AST_SymbolLambda"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolLambda (props)](#apidoc.element.uglify-js.AST_SymbolLambda.AST_SymbolLambda)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolLambda.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolLambda.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolLambda.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolLambda.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolLambda.prototype"></a>[module uglify-js.AST_SymbolLambda.prototype](#apidoc.module.uglify-js.AST_SymbolLambda.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolLambda.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolLambda.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolLambda.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolRef"></a>[module uglify-js.AST_SymbolRef](#apidoc.module.uglify-js.AST_SymbolRef)

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.AST_SymbolRef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolRef (props)](#apidoc.element.uglify-js.AST_SymbolRef.AST_SymbolRef)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolRef.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolRef.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolRef.prototype"></a>[module uglify-js.AST_SymbolRef.prototype](#apidoc.module.uglify-js.AST_SymbolRef.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_SymbolRef.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    if (this._evaluating) throw def;
    this._evaluating = true;
    try {
        var d = this.definition();
        if (compressor.option("reduce_vars") && d.fixed) {
            if (compressor.option("unsafe")) {
                if (!HOP(d.fixed, "_evaluated")) {
                    d.fixed._evaluated = ev(d.fixed, compressor);
                }
                return d.fixed._evaluated;
            }
            return ev(d.fixed, compressor);
        }
    } finally {
        this._evaluating = false;
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.prototype._find_defs"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>_find_defs (compressor, suffix)](#apidoc.element.uglify-js.AST_SymbolRef.prototype._find_defs)
- description and source-code
```javascript
_find_defs = function (compressor, suffix){
    if (!this.global()) return;
    var name;
    var defines = compressor.option("global_defs");
    if (defines && HOP(defines, (name = this.name + suffix))) {
        var node = to_node(defines[name], this);
        var top = compressor.find_parent(AST_Toplevel);
        node.walk(new TreeWalker(function(node) {
            if (node instanceof AST_SymbolRef) {
                node.scope = top;
                node.thedef = top.def_global(node);
            }
        }));
        return node;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_SymbolRef.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function () {
    return this.undeclared() ? this : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.global() && this.undeclared();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolRef.prototype.reference"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolRef.prototype.</span>reference (options)](#apidoc.element.uglify-js.AST_SymbolRef.prototype.reference)
- description and source-code
```javascript
reference = function (options) {
    var def = this.definition();
    def.references.push(this);
    var s = this.scope;
    while (s) {
        push_uniq(s.enclosed, def);
        if (options.keep_fnames) {
            s.functions.each(function(d) {
                push_uniq(def.scope.enclosed, d);
            });
        }
        if (s === def.scope) break;
        s = s.parent_scope;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolVar"></a>[module uglify-js.AST_SymbolVar](#apidoc.module.uglify-js.AST_SymbolVar)

#### <a name="apidoc.element.uglify-js.AST_SymbolVar.AST_SymbolVar"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_SymbolVar (props)](#apidoc.element.uglify-js.AST_SymbolVar.AST_SymbolVar)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolVar.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>BASE (props)](#apidoc.element.uglify-js.AST_SymbolVar.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_SymbolVar.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_SymbolVar.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolVar.SUBCLASSES"></a>[module uglify-js.AST_SymbolVar.SUBCLASSES](#apidoc.module.uglify-js.AST_SymbolVar.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_SymbolVar.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_SymbolVar.SUBCLASSES.0)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_SymbolVar.prototype"></a>[module uglify-js.AST_SymbolVar.prototype](#apidoc.module.uglify-js.AST_SymbolVar.prototype)

#### <a name="apidoc.element.uglify-js.AST_SymbolVar.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_SymbolVar.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_SymbolVar.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_This"></a>[module uglify-js.AST_This](#apidoc.module.uglify-js.AST_This)

#### <a name="apidoc.element.uglify-js.AST_This.AST_This"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_This (props)](#apidoc.element.uglify-js.AST_This.AST_This)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_This.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_This.</span>BASE (props)](#apidoc.element.uglify-js.AST_This.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_This.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_This.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_This.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_This.prototype"></a>[module uglify-js.AST_This.prototype](#apidoc.module.uglify-js.AST_This.prototype)

#### <a name="apidoc.element.uglify-js.AST_This.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_This.prototype.CTOR)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_This.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_This.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("this");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_This.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>drop_side_effect_free ()](#apidoc.element.uglify-js.AST_This.prototype.drop_side_effect_free)
- description and source-code
```javascript
function return_null() { return null; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_This.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>has_side_effects ()](#apidoc.element.uglify-js.AST_This.prototype.has_side_effects)
- description and source-code
```javascript
function return_false() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_This.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_This.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_This.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Throw"></a>[module uglify-js.AST_Throw](#apidoc.module.uglify-js.AST_Throw)

#### <a name="apidoc.element.uglify-js.AST_Throw.AST_Throw"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Throw (props)](#apidoc.element.uglify-js.AST_Throw.AST_Throw)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Throw.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>BASE (props)](#apidoc.element.uglify-js.AST_Throw.BASE)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Throw.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Throw.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Throw.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Throw.prototype"></a>[module uglify-js.AST_Throw.prototype](#apidoc.module.uglify-js.AST_Throw.prototype)

#### <a name="apidoc.element.uglify-js.AST_Throw.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Throw.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Throw.prototype.CTOR)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Throw.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Throw.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Throw.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "throw");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Throw.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Throw.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Throw.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_Token"></a>[module uglify-js.AST_Token](#apidoc.module.uglify-js.AST_Token)

#### <a name="apidoc.element.uglify-js.AST_Token.AST_Token"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Token (props)](#apidoc.element.uglify-js.AST_Token.AST_Token)
- description and source-code
```javascript
function AST_Token(props){ if (props) { this.raw = props.raw;this.file = props.file;this.comments_before = props.comments_before
;this.nlb = props.nlb;this.endpos = props.endpos;this.endcol = props.endcol;this.endline = props.endline;this.pos = props.pos;this
.col = props.col;this.line = props.line;this.value = props.value;this.type = props.type;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Token.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Token.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Token.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Token.prototype"></a>[module uglify-js.AST_Token.prototype](#apidoc.module.uglify-js.AST_Token.prototype)

#### <a name="apidoc.element.uglify-js.AST_Token.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Token.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Token.prototype.CTOR)
- description and source-code
```javascript
function AST_Token(props){ if (props) { this.raw = props.raw;this.file = props.file;this.comments_before = props.comments_before
;this.nlb = props.nlb;this.endpos = props.endpos;this.endcol = props.endcol;this.endline = props.endline;this.pos = props.pos;this
.col = props.col;this.line = props.line;this.value = props.value;this.type = props.type;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Toplevel"></a>[module uglify-js.AST_Toplevel](#apidoc.module.uglify-js.AST_Toplevel)

#### <a name="apidoc.element.uglify-js.AST_Toplevel.AST_Toplevel"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Toplevel (props)](#apidoc.element.uglify-js.AST_Toplevel.AST_Toplevel)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>BASE (props)](#apidoc.element.uglify-js.AST_Toplevel.BASE)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Toplevel.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Toplevel.prototype"></a>[module uglify-js.AST_Toplevel.prototype](#apidoc.module.uglify-js.AST_Toplevel.prototype)

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Toplevel.prototype.CTOR)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Toplevel.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    display_body(self.body, true, output, true);
    output.print("");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype._default_mangler_options"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>_default_mangler_options (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype._default_mangler_options)
- description and source-code
```javascript
_default_mangler_options = function (options){
    return defaults(options, {
        except      : [],
        eval        : false,
        sort        : false, // Ignored. Flag retained for backwards compatibility.
        toplevel    : false,
        screw_ie8   : true,
        keep_fnames : false
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Toplevel.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.compute_char_frequency"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>compute_char_frequency (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.compute_char_frequency)
- description and source-code
```javascript
compute_char_frequency = function (options){
    options = this._default_mangler_options(options);
    var tw = new TreeWalker(function(node){
        if (node instanceof AST_Constant)
            base54.consider(node.print_to_string());
        else if (node instanceof AST_Return)
            base54.consider("return");
        else if (node instanceof AST_Throw)
            base54.consider("throw");
        else if (node instanceof AST_Continue)
            base54.consider("continue");
        else if (node instanceof AST_Break)
            base54.consider("break");
        else if (node instanceof AST_Debugger)
            base54.consider("debugger");
        else if (node instanceof AST_Directive)
            base54.consider(node.value);
        else if (node instanceof AST_While)
            base54.consider("while");
        else if (node instanceof AST_Do)
            base54.consider("do while");
        else if (node instanceof AST_If) {
            base54.consider("if");
            if (node.alternative) base54.consider("else");
        }
        else if (node instanceof AST_Var)
            base54.consider("var");
        else if (node instanceof AST_Const)
            base54.consider("const");
        else if (node instanceof AST_Lambda)
            base54.consider("function");
        else if (node instanceof AST_For)
            base54.consider("for");
        else if (node instanceof AST_ForIn)
            base54.consider("for in");
        else if (node instanceof AST_Switch)
            base54.consider("switch");
        else if (node instanceof AST_Case)
            base54.consider("case");
        else if (node instanceof AST_Default)
            base54.consider("default");
        else if (node instanceof AST_With)
            base54.consider("with");
        else if (node instanceof AST_ObjectSetter)
            base54.consider("set" + node.key);
        else if (node instanceof AST_ObjectGetter)
            base54.consider("get" + node.key);
        else if (node instanceof AST_ObjectKeyVal)
            base54.consider(node.key);
        else if (node instanceof AST_New)
            base54.consider("new");
        else if (node instanceof AST_This)
            base54.consider("this");
        else if (node instanceof AST_Try)
            base54.consider("try");
        else if (node instanceof AST_Catch)
            base54.consider("catch");
        else if (node instanceof AST_Finally)
            base54.consider("finally");
        else if (node instanceof AST_Symbol && node.unmangleable(options))
            base54.consider(node.name);
        else if (node instanceof AST_Unary || node instanceof AST_Binary)
            base54.consider(node.operator);
        else if (node instanceof AST_Dot)
            base54.consider(node.property);
    });
    this.walk(tw);
    base54.sort();
}
```
- example usage
```shell
...
  // Compression
  uAST.figure_out_scope();
  uAST = UglifyJS.Compressor(options).compress(uAST);

  // Mangling (optional)
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''
...
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.def_global"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>def_global (node)](#apidoc.element.uglify-js.AST_Toplevel.prototype.def_global)
- description and source-code
```javascript
def_global = function (node){
    var globals = this.globals, name = node.name;
    if (globals.has(name)) {
        return globals.get(name);
    } else {
        var g = new SymbolDef(this, globals.size(), node);
        g.undeclared = true;
        g.global = true;
        globals.set(name, g);
        return g;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.figure_out_scope"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>figure_out_scope (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.figure_out_scope)
- description and source-code
```javascript
figure_out_scope = function (options){
    options = defaults(options, {
        screw_ie8: true,
        cache: null
    });

    // pass 1: setup scope chaining and handle definitions
    var self = this;
    var scope = self.parent_scope = null;
    var labels = new Dictionary();
    var defun = null;
    var tw = new TreeWalker(function(node, descend){
        if (node instanceof AST_Catch) {
            var save_scope = scope;
            scope = new AST_Scope(node);
            scope.init_scope_vars();
            scope.parent_scope = save_scope;
            descend();
            scope = save_scope;
            return true;
        }
        if (node instanceof AST_Scope) {
            node.init_scope_vars();
            var save_scope = node.parent_scope = scope;
            var save_defun = defun;
            var save_labels = labels;
            defun = scope = node;
            labels = new Dictionary();
            descend();
            scope = save_scope;
            defun = save_defun;
            labels = save_labels;
            return true;        // don't descend again in TreeWalker
        }
        if (node instanceof AST_LabeledStatement) {
            var l = node.label;
            if (labels.has(l.name)) {
                throw new Error(string_template("Label {name} defined twice", l));
            }
            labels.set(l.name, l);
            descend();
            labels.del(l.name);
            return true;        // no descend again
        }
        if (node instanceof AST_With) {
            for (var s = scope; s; s = s.parent_scope)
                s.uses_with = true;
            return;
        }
        if (node instanceof AST_Symbol) {
            node.scope = scope;
        }
        if (node instanceof AST_Label) {
            node.thedef = node;
            node.references = [];
        }
        if (node instanceof AST_SymbolLambda) {
            defun.def_function(node);
        }
        else if (node instanceof AST_SymbolDefun) {
            // Careful here, the scope where this should be defined is
            // the parent scope.  The reason is that we enter a new
            // scope when we encounter the AST_Defun node (which is
            // instanceof AST_Scope) but we get to the symbol a bit
            // later.
            (node.scope = defun.parent_scope).def_function(node);
        }
        else if (node instanceof AST_SymbolVar
                 || node instanceof AST_SymbolConst) {
            defun.def_variable(node);
        }
        else if (node instanceof AST_SymbolCatch) {
            scope.def_variable(node);
        }
        else if (node instanceof AST_LabelRef) {
            var sym = labels.get(node.name);
            if (!sym) throw new Error(string_template("Undefined label {name} [{line},{col}]", {
                name: node.name,
                line: node.start.line,
                col: node.start.col
            }));
            node.thedef = sym;
        }
    });
    self.walk(tw);

    // pass 2: find back references and eval
    var func = null;
    var globals = self.globals = new Dictionary();
    var tw = new TreeWalker(function(node, descend){
        if (node instanceof AST_Lambda) {
            var prev_func = func;
            func = node;
            descend();
            func = prev_func;
            return true;
        }
        if (node instanceof AST_LoopControl && node.label) {
            node.label.thedef.references.push(node);
            return true;
        }
        if (node instanceof AST_SymbolRef) {
            var name = node.name;
            if (name == "eval" && tw.parent() instanceof AST_Call) {
                for (var s = node.scope; s && !s.uses_eval; s = s.parent_scope) {
                    s.uses_eval = true;
                }
            }
            var sym = node.scope.find_variable(name);
            if (node.scope instanceof AST_Lambda && name == "arguments") {
                node.scope.uses_arguments = true;
            }
            if (!sym) {
                sym = self.def_global(node);
            } ...
```
- example usage
```shell
...

'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = UglifyJS.Compressor(options).compress(uAST);

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
...
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.mangle_names"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>mangle_names (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.mangle_names)
- description and source-code
```javascript
mangle_names = function (options){
    options = this._default_mangler_options(options);

    // Never mangle arguments
    options.except.push('arguments');

    // We only need to mangle declaration nodes.  Special logic wired
    // into the code generator will display the mangled name if it's
    // present (and for AST_SymbolRef-s it'll use the mangled name of
    // the AST_SymbolDeclaration that it points to).
    var lname = -1;
    var to_mangle = [];

    if (options.cache) {
        this.globals.each(function(symbol){
            if (options.except.indexOf(symbol.name) < 0) {
                to_mangle.push(symbol);
            }
        });
    }

    var tw = new TreeWalker(function(node, descend){
        if (node instanceof AST_LabeledStatement) {
            // lname is incremented when we get to the AST_Label
            var save_nesting = lname;
            descend();
            lname = save_nesting;
            return true;        // don't descend again in TreeWalker
        }
        if (node instanceof AST_Scope) {
            var p = tw.parent(), a = [];
            node.variables.each(function(symbol){
                if (options.except.indexOf(symbol.name) < 0) {
                    a.push(symbol);
                }
            });
            to_mangle.push.apply(to_mangle, a);
            return;
        }
        if (node instanceof AST_Label) {
            var name;
            do name = base54(++lname); while (!is_identifier(name));
            node.mangled_name = name;
            return true;
        }
        if (options.screw_ie8 && node instanceof AST_SymbolCatch) {
            to_mangle.push(node.definition());
            return;
        }
    });
    this.walk(tw);
    to_mangle.forEach(function(def){ def.mangle(options) });

    if (options.cache) {
        options.cache.cname = this.cname;
    }
}
```
- example usage
```shell
...
  uAST.figure_out_scope();
  uAST = UglifyJS.Compressor(options).compress(uAST);

  // Mangling (optional)
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''
...
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.scope_warnings"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>scope_warnings (options)](#apidoc.element.uglify-js.AST_Toplevel.prototype.scope_warnings)
- description and source-code
```javascript
scope_warnings = function (options){
    options = defaults(options, {
        undeclared       : false, // this makes a lot of noise
        unreferenced     : true,
        assign_to_global : true,
        func_arguments   : true,
        nested_defuns    : true,
        eval             : true
    });
    var tw = new TreeWalker(function(node){
        if (options.undeclared
            && node instanceof AST_SymbolRef
            && node.undeclared())
        {
            // XXX: this also warns about JS standard names,
            // i.e. Object, Array, parseInt etc.  Should add a list of
            // exceptions.
            AST_Node.warn("Undeclared symbol: {name} [{file}:{line},{col}]", {
                name: node.name,
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
        if (options.assign_to_global)
        {
            var sym = null;
            if (node instanceof AST_Assign && node.left instanceof AST_SymbolRef)
                sym = node.left;
            else if (node instanceof AST_ForIn && node.init instanceof AST_SymbolRef)
                sym = node.init;
            if (sym
                && (sym.undeclared()
                    || (sym.global() && sym.scope !== sym.definition().scope))) {
                AST_Node.warn("{msg}: {name} [{file}:{line},{col}]", {
                    msg: sym.undeclared() ? "Accidental global?" : "Assignment to global",
                    name: sym.name,
                    file: sym.start.file,
                    line: sym.start.line,
                    col: sym.start.col
                });
            }
        }
        if (options.eval
            && node instanceof AST_SymbolRef
            && node.undeclared()
            && node.name == "eval") {
            AST_Node.warn("Eval is used [{file}:{line},{col}]", node.start);
        }
        if (options.unreferenced
            && (node instanceof AST_SymbolDeclaration || node instanceof AST_Label)
            && !(node instanceof AST_SymbolCatch)
            && node.unreferenced()) {
            AST_Node.warn("{type} {name} is declared but not referenced [{file}:{line},{col}]", {
                type: node instanceof AST_Label ? "Label" : "Symbol",
                name: node.name,
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
        if (options.func_arguments
            && node instanceof AST_Lambda
            && node.uses_arguments) {
            AST_Node.warn("arguments used in function {name} [{file}:{line},{col}]", {
                name: node.name ? node.name.name : "anonymous",
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
        if (options.nested_defuns
            && node instanceof AST_Defun
            && !(tw.parent() instanceof AST_Scope)) {
            AST_Node.warn("Function {name} declared in nested statement \"{type}\" [{file}:{line},{col}]", {
                name: node.name.name,
                type: tw.parent().TYPE,
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
    });
    this.walk(tw);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Toplevel.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.wrap_commonjs"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>wrap_commonjs (name, export_all)](#apidoc.element.uglify-js.AST_Toplevel.prototype.wrap_commonjs)
- description and source-code
```javascript
wrap_commonjs = function (name, export_all) {
    var self = this;
    var to_export = [];
    if (export_all) {
        self.figure_out_scope();
        self.walk(new TreeWalker(function(node){
            if (node instanceof AST_SymbolDeclaration && node.definition().global) {
                if (!find_if(function(n){ return n.name == node.name }, to_export))
                    to_export.push(node);
            }
        }));
    }
    var wrapped_tl = "(function(exports, global){ '$ORIG'; '$EXPORTS'; global['" + name + "'] = exports; }({}, (function(){return
 this}())))";
    wrapped_tl = parse(wrapped_tl);
    wrapped_tl = wrapped_tl.transform(new TreeTransformer(function before(node){
        if (node instanceof AST_Directive) {
            switch (node.value) {
              case "$ORIG":
                return MAP.splice(self.body);
              case "$EXPORTS":
                var body = [];
                to_export.forEach(function(sym){
                    body.push(new AST_SimpleStatement({
                        body: new AST_Assign({
                            left: new AST_Sub({
                                expression: new AST_SymbolRef({ name: "exports" }),
                                property: new AST_String({ value: sym.name }),
                            }),
                            operator: "=",
                            right: new AST_SymbolRef(sym),
                        }),
                    }));
                });
                return MAP.splice(body);
            }
        }
    }));
    return wrapped_tl;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Toplevel.prototype.wrap_enclose"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Toplevel.prototype.</span>wrap_enclose (arg_parameter_pairs)](#apidoc.element.uglify-js.AST_Toplevel.prototype.wrap_enclose)
- description and source-code
```javascript
wrap_enclose = function (arg_parameter_pairs) {
    var self = this;
    var args = [];
    var parameters = [];

    arg_parameter_pairs.forEach(function(pair) {
        var splitAt = pair.lastIndexOf(":");

        args.push(pair.substr(0, splitAt));
        parameters.push(pair.substr(splitAt + 1));
    });

    var wrapped_tl = "(function(" + parameters.join(",") + "){ '$ORIG'; })(" + args.join(",") + ")";
    wrapped_tl = parse(wrapped_tl);
    wrapped_tl = wrapped_tl.transform(new TreeTransformer(function before(node){
        if (node instanceof AST_Directive && node.value == "$ORIG") {
            return MAP.splice(self.body);
        }
    }));
    return wrapped_tl;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_True"></a>[module uglify-js.AST_True](#apidoc.module.uglify-js.AST_True)

#### <a name="apidoc.element.uglify-js.AST_True.AST_True"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_True (props)](#apidoc.element.uglify-js.AST_True.AST_True)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_True.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_True.</span>BASE (props)](#apidoc.element.uglify-js.AST_True.BASE)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_True.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_True.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_True.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_True.prototype"></a>[module uglify-js.AST_True.prototype](#apidoc.module.uglify-js.AST_True.prototype)

#### <a name="apidoc.element.uglify-js.AST_True.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_True.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_True.prototype.CTOR)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_True.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_True.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_True.prototype.is_boolean)
- description and source-code
```javascript
function return_true() { return true; }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Try"></a>[module uglify-js.AST_Try](#apidoc.module.uglify-js.AST_Try)

#### <a name="apidoc.element.uglify-js.AST_Try.AST_Try"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Try (props)](#apidoc.element.uglify-js.AST_Try.AST_Try)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>BASE (props)](#apidoc.element.uglify-js.AST_Try.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Try.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Try.prototype"></a>[module uglify-js.AST_Try.prototype](#apidoc.module.uglify-js.AST_Try.prototype)

#### <a name="apidoc.element.uglify-js.AST_Try.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Try.prototype.CTOR)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Try.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("try");
    output.space();
    print_bracketed(self.body, output);
    if (self.bcatch) {
        output.space();
        self.bcatch.print(output);
    }
    if (self.bfinally) {
        output.space();
        self.bfinally.print(output);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Try.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        walk_body(this, visitor);
        if (this.bcatch) this.bcatch._walk(visitor);
        if (this.bfinally) this.bfinally._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>add_source_map (stream)](#apidoc.element.uglify-js.AST_Try.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Try.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Try.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Try.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Try.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Try.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Try.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_Unary"></a>[module uglify-js.AST_Unary](#apidoc.module.uglify-js.AST_Unary)

#### <a name="apidoc.element.uglify-js.AST_Unary.AST_Unary"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Unary (props)](#apidoc.element.uglify-js.AST_Unary.AST_Unary)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>BASE (props)](#apidoc.element.uglify-js.AST_Unary.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Unary.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Unary.SUBCLASSES"></a>[module uglify-js.AST_Unary.SUBCLASSES](#apidoc.module.uglify-js.AST_Unary.SUBCLASSES)

#### <a name="apidoc.element.uglify-js.AST_Unary.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglify-js.AST_Unary.SUBCLASSES.0)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.SUBCLASSES.</span>1 (props)](#apidoc.element.uglify-js.AST_Unary.SUBCLASSES.1)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Unary.prototype"></a>[module uglify-js.AST_Unary.prototype](#apidoc.module.uglify-js.AST_Unary.prototype)

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Unary.prototype.CTOR)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_Unary.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.drop_side_effect_free"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>drop_side_effect_free (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_Unary.prototype.drop_side_effect_free)
- description and source-code
```javascript
drop_side_effect_free = function (compressor, first_in_statement){
    switch (this.operator) {
      case "delete":
      case "++":
      case "--":
        return this;
      case "typeof":
        if (this.expression instanceof AST_SymbolRef) return null;
      default:
        var expression = this.expression.drop_side_effect_free(compressor, first_in_statement);
        if (first_in_statement
            && this instanceof AST_UnaryPrefix
            && is_iife_call(expression)) {
            if (expression === this.expression && this.operator.length === 1) return this;
            return make_node(AST_UnaryPrefix, this, {
                operator: this.operator.length === 1 ? this.operator : "!",
                expression: expression
            });
        }
        return expression;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglify-js.AST_Unary.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.operator == "delete"
        || this.operator == "++"
        || this.operator == "--"
        || this.expression.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.is_number"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>is_number ()](#apidoc.element.uglify-js.AST_Unary.prototype.is_number)
- description and source-code
```javascript
is_number = function (){
    return unary(this.operator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.lift_sequences"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglify-js.AST_Unary.prototype.lift_sequences)
- description and source-code
```javascript
lift_sequences = function (compressor){
    if (compressor.option("sequences")) {
        if (this.expression instanceof AST_Seq) {
            var seq = this.expression;
            var x = seq.to_array();
            this.expression = x.pop();
            x.push(this);
            seq = AST_Seq.from_array(x).transform(compressor);
            return seq;
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Unary.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    return p instanceof AST_PropAccess && p.expression === this
        || p instanceof AST_Call && p.expression === this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_Unary.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_Unary.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Unary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_Unary.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_UnaryPostfix"></a>[module uglify-js.AST_UnaryPostfix](#apidoc.module.uglify-js.AST_UnaryPostfix)

#### <a name="apidoc.element.uglify-js.AST_UnaryPostfix.AST_UnaryPostfix"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPostfix (props)](#apidoc.element.uglify-js.AST_UnaryPostfix.AST_UnaryPostfix)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPostfix.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>BASE (props)](#apidoc.element.uglify-js.AST_UnaryPostfix.BASE)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPostfix.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_UnaryPostfix.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_UnaryPostfix.prototype"></a>[module uglify-js.AST_UnaryPostfix.prototype](#apidoc.module.uglify-js.AST_UnaryPostfix.prototype)

#### <a name="apidoc.element.uglify-js.AST_UnaryPostfix.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_UnaryPostfix.prototype.CTOR)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPostfix.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_UnaryPostfix.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.expression.print(output);
    output.print(self.operator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPostfix.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPostfix.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_UnaryPostfix.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_UnaryPrefix"></a>[module uglify-js.AST_UnaryPrefix](#apidoc.module.uglify-js.AST_UnaryPrefix)

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.AST_UnaryPrefix"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_UnaryPrefix (props)](#apidoc.element.uglify-js.AST_UnaryPrefix.AST_UnaryPrefix)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>BASE (props)](#apidoc.element.uglify-js.AST_UnaryPrefix.BASE)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_UnaryPrefix.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_UnaryPrefix.prototype"></a>[module uglify-js.AST_UnaryPrefix.prototype](#apidoc.module.uglify-js.AST_UnaryPrefix.prototype)

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.CTOR)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var op = self.operator;
    output.print(op);
    if (/^[a-z]/i.test(op)
        || (/[+-]$/.test(op)
            && self.expression instanceof AST_UnaryPrefix
            && /^[+-]/.test(self.expression.operator))) {
        output.space();
    }
    self.expression.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>_eval (compressor)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    var e = this.expression;
    switch (this.operator) {
      case "!": return !ev(e, compressor);
      case "typeof":
        // Function would be evaluated to an array and so typeof would
        // incorrectly return 'object'. Hence making is a special case.
        if (e instanceof AST_Function) return typeof function(){};

        e = ev(e, compressor);

        // typeof <RegExp> returns "object" or "function" on different platforms
        // so cannot evaluate reliably
        if (e instanceof RegExp) throw def;

        return typeof e;
      case "void": return void ev(e, compressor);
      case "~": return ~ev(e, compressor);
      case "-": return -ev(e, compressor);
      case "+": return +ev(e, compressor);
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>is_boolean ()](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return member(this.operator, unary_bool);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>is_string ()](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.is_string)
- description and source-code
```javascript
is_string = function (){
    return this.operator == "typeof";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>negate (compressor, first_in_statement)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.negate)
- description and source-code
```javascript
negate = function (compressor, first_in_statement){
    return func.call(this, compressor, first_in_statement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_UnaryPrefix.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_UnaryPrefix.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_UnaryPrefix.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Undefined"></a>[module uglify-js.AST_Undefined](#apidoc.module.uglify-js.AST_Undefined)

#### <a name="apidoc.element.uglify-js.AST_Undefined.AST_Undefined"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Undefined (props)](#apidoc.element.uglify-js.AST_Undefined.AST_Undefined)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Undefined.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>BASE (props)](#apidoc.element.uglify-js.AST_Undefined.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Undefined.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Undefined.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Undefined.prototype"></a>[module uglify-js.AST_Undefined.prototype](#apidoc.module.uglify-js.AST_Undefined.prototype)

#### <a name="apidoc.element.uglify-js.AST_Undefined.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Undefined.prototype.CTOR)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Undefined.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Undefined.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("void 0");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Undefined.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>needs_parens (output)](#apidoc.element.uglify-js.AST_Undefined.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    return p instanceof AST_PropAccess && p.expression === this
        || p instanceof AST_Call && p.expression === this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Undefined.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Undefined.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_Undefined.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Var"></a>[module uglify-js.AST_Var](#apidoc.module.uglify-js.AST_Var)

#### <a name="apidoc.element.uglify-js.AST_Var.AST_Var"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_Var (props)](#apidoc.element.uglify-js.AST_Var.AST_Var)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Var.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>BASE (props)](#apidoc.element.uglify-js.AST_Var.BASE)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Var.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Var.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_Var.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_Var.prototype"></a>[module uglify-js.AST_Var.prototype](#apidoc.module.uglify-js.AST_Var.prototype)

#### <a name="apidoc.element.uglify-js.AST_Var.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Var.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_Var.prototype.CTOR)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_Var.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_Var.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_Var.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "var");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_VarDef"></a>[module uglify-js.AST_VarDef](#apidoc.module.uglify-js.AST_VarDef)

#### <a name="apidoc.element.uglify-js.AST_VarDef.AST_VarDef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_VarDef (props)](#apidoc.element.uglify-js.AST_VarDef.AST_VarDef)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_VarDef.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>BASE (props)](#apidoc.element.uglify-js.AST_VarDef.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_VarDef.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_VarDef.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_VarDef.prototype"></a>[module uglify-js.AST_VarDef.prototype](#apidoc.module.uglify-js.AST_VarDef.prototype)

#### <a name="apidoc.element.uglify-js.AST_VarDef.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_VarDef.prototype.CTOR)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_VarDef.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_VarDef.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.name.print(output);
    if (self.value) {
        output.space();
        output.print("=");
        output.space();
        var p = output.parent(1);
        var noin = p instanceof AST_For || p instanceof AST_ForIn;
        parenthesize_for_noin(self.value, output, noin);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_VarDef.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_VarDef.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.name._walk(visitor);
        if (this.value) this.value._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_VarDef.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>optimize (compressor)](#apidoc.element.uglify-js.AST_VarDef.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    if (compressor.has_directive("use asm")) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_VarDef.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_VarDef.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_VarDef.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_VarDef.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_VarDef.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.AST_While"></a>[module uglify-js.AST_While](#apidoc.module.uglify-js.AST_While)

#### <a name="apidoc.element.uglify-js.AST_While.AST_While"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_While (props)](#apidoc.element.uglify-js.AST_While.AST_While)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_While.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_While.</span>BASE (props)](#apidoc.element.uglify-js.AST_While.BASE)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_While.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_While.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_While.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_While.prototype"></a>[module uglify-js.AST_While.prototype](#apidoc.module.uglify-js.AST_While.prototype)

#### <a name="apidoc.element.uglify-js.AST_While.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_While.prototype.CTOR)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_While.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_While.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("while");
    output.space();
    output.with_parens(function(){
        self.condition.print(output);
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_While.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_While.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.condition._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_While.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_While.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_While.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglify-js.AST_With"></a>[module uglify-js.AST_With](#apidoc.module.uglify-js.AST_With)

#### <a name="apidoc.element.uglify-js.AST_With.AST_With"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>AST_With (props)](#apidoc.element.uglify-js.AST_With.AST_With)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_With.BASE"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_With.</span>BASE (props)](#apidoc.element.uglify-js.AST_With.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_With.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_With.</span>DEFMETHOD (name, method)](#apidoc.element.uglify-js.AST_With.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.AST_With.prototype"></a>[module uglify-js.AST_With.prototype](#apidoc.module.uglify-js.AST_With.prototype)

#### <a name="apidoc.element.uglify-js.AST_With.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>CTOR (props)](#apidoc.element.uglify-js.AST_With.prototype.CTOR)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_With.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>_codegen (self, output)](#apidoc.element.uglify-js.AST_With.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("with");
    output.space();
    output.with_parens(function(){
        self.expression.print(output);
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_With.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>_walk (visitor)](#apidoc.element.uglify-js.AST_With.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.AST_With.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglify-js.AST_With.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglify-js.AST_With.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglify-js.AST_With.prototype.</span>transform (tw, in_list)](#apidoc.element.uglify-js.AST_With.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this;
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop(this);
    return x;
}
```
- example usage
```shell
...
    }
    else if (node instanceof AST_Sub) {
        addStrings(node.property, ignore_quoted);
    }
}));

// step 2: transform the tree, renaming properties
return ast.transform(new TreeTransformer(function(node){
    if (node instanceof AST_ObjectKeyVal) {
        if (!(ignore_quoted && node.quote))
            node.key = mangle(node.key);
    }
    else if (node instanceof AST_ObjectProperty) {
        // setter or getter
        node.key.name = mangle(node.key.name);
...
```



# <a name="apidoc.module.uglify-js.Compressor"></a>[module uglify-js.Compressor](#apidoc.module.uglify-js.Compressor)

#### <a name="apidoc.element.uglify-js.Compressor.Compressor"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>Compressor (options, false_by_default)](#apidoc.element.uglify-js.Compressor.Compressor)
- description and source-code
```javascript
function Compressor(options, false_by_default) {
    if (!(this instanceof Compressor))
        return new Compressor(options, false_by_default);
    TreeTransformer.call(this, this.before, this.after);
    this.options = defaults(options, {
        sequences     : !false_by_default,
        properties    : !false_by_default,
        dead_code     : !false_by_default,
        drop_debugger : !false_by_default,
        unsafe        : false,
        unsafe_comps  : false,
        unsafe_math   : false,
        unsafe_proto  : false,
        conditionals  : !false_by_default,
        comparisons   : !false_by_default,
        evaluate      : !false_by_default,
        booleans      : !false_by_default,
        loops         : !false_by_default,
        unused        : !false_by_default,
        toplevel      : !!(options && options["top_retain"]),
        top_retain    : null,
        hoist_funs    : !false_by_default,
        keep_fargs    : true,
        keep_fnames   : false,
        hoist_vars    : false,
        if_return     : !false_by_default,
        join_vars     : !false_by_default,
        collapse_vars : !false_by_default,
        reduce_vars   : !false_by_default,
        cascade       : !false_by_default,
        side_effects  : !false_by_default,
        pure_getters  : false,
        pure_funcs    : null,
        negate_iife   : !false_by_default,
        screw_ie8     : true,
        drop_console  : false,
        angular       : false,
        expression    : false,
        warnings      : true,
        global_defs   : {},
        passes        : 1,
    }, true);
    var pure_funcs = this.options["pure_funcs"];
    if (typeof pure_funcs == "function") {
        this.pure_funcs = pure_funcs;
    } else {
        this.pure_funcs = pure_funcs ? function(node) {
            return pure_funcs.indexOf(node.expression.print_to_string()) < 0;
        } : return_true;
    }
    var top_retain = this.options["top_retain"];
    if (top_retain instanceof RegExp) {
        this.top_retain = function(def) {
            return top_retain.test(def.name);
        };
    } else if (typeof top_retain == "function") {
        this.top_retain = top_retain;
    } else if (top_retain) {
        if (typeof top_retain == "string") {
            top_retain = top_retain.split(/,/);
        }
        this.top_retain = function(def) {
            return top_retain.indexOf(def.name) >= 0;
        };
    }
    var sequences = this.options["sequences"];
    this.sequences_limit = sequences == 1 ? 200 : sequences | 0;
    this.warnings_produced = {};
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = UglifyJS.Compressor(options).compress(uAST);

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglify-js.Compressor.prototype"></a>[module uglify-js.Compressor.prototype](#apidoc.module.uglify-js.Compressor.prototype)

#### <a name="apidoc.element.uglify-js.Compressor.prototype.before"></a>[function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>before (node, descend, in_list)](#apidoc.element.uglify-js.Compressor.prototype.before)
- description and source-code
```javascript
before = function (node, descend, in_list) {
    if (node._squeezed) return node;
    var was_scope = false;
    if (node instanceof AST_Scope) {
        node = node.hoist_declarations(this);
        was_scope = true;
    }
    // Before https://github.com/mishoo/UglifyJS2/pull/1602 AST_Node.optimize()
    // would call AST_Node.transform() if a different instance of AST_Node is
    // produced after OPT().
    // This corrupts TreeWalker.stack, which cause AST look-ups to malfunction.
    // Migrate and defer all children's AST_Node.transform() to below, which
    // will now happen after this parent AST_Node has been properly substituted
    // thus gives a consistent AST snapshot.
    descend(node, this);
    // Existing code relies on how AST_Node.optimize() worked, and omitting the
    // following replacement call would result in degraded efficiency of both
    // output and performance.
    descend(node, this);
    var opt = node.optimize(this);
    if (was_scope && opt instanceof AST_Scope) {
        opt.drop_unused(this);
        descend(opt, this);
    }
    if (opt === node) opt._squeezed = true;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Compressor.prototype.clear_warnings"></a>[function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>clear_warnings ()](#apidoc.element.uglify-js.Compressor.prototype.clear_warnings)
- description and source-code
```javascript
clear_warnings = function () {
    this.warnings_produced = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Compressor.prototype.compress"></a>[function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>compress (node)](#apidoc.element.uglify-js.Compressor.prototype.compress)
- description and source-code
```javascript
compress = function (node) {
    if (this.option("expression")) {
        node = node.process_expression(true);
    }
    var passes = +this.options.passes || 1;
    for (var pass = 0; pass < passes && pass < 3; ++pass) {
        if (pass > 0 || this.option("reduce_vars"))
            node.reset_opt_flags(this, true);
        node = node.transform(this);
    }
    if (this.option("expression")) {
        node = node.process_expression(false);
    }
    return node;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = UglifyJS.Compressor(options).compress(uAST);

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```

#### <a name="apidoc.element.uglify-js.Compressor.prototype.info"></a>[function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>info ()](#apidoc.element.uglify-js.Compressor.prototype.info)
- description and source-code
```javascript
info = function () {
    if (this.options.warnings == "verbose") {
        AST_Node.warn.apply(AST_Node, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Compressor.prototype.option"></a>[function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>option (key)](#apidoc.element.uglify-js.Compressor.prototype.option)
- description and source-code
```javascript
option = function (key) { return this.options[key] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Compressor.prototype.warn"></a>[function <span class="apidocSignatureSpan">uglify-js.Compressor.prototype.</span>warn (text, props)](#apidoc.element.uglify-js.Compressor.prototype.warn)
- description and source-code
```javascript
warn = function (text, props) {
    if (this.options.warnings) {
        // only emit unique warnings
        var message = string_template(text, props);
        if (!(message in this.warnings_produced)) {
            this.warnings_produced[message] = true;
            AST_Node.warn.apply(AST_Node, arguments);
        }
    }
}
```
- example usage
```shell
...
}
else if (node instanceof AST_Sub) {
    if (!ignore_quoted)
        node.property = mangleStrings(node.property);
}
// else if (node instanceof AST_String) {
//     if (should_mangle(node.value)) {
//         AST_Node.warn(
//             "Found \"{prop}\" property candidate for mangling in an arbitrary string [{file}:{line},{col}]", {
//                 file : node.start.file,
//                 line : node.start.line,
//                 col  : node.start.col,
//                 prop : node.value
//             }
//         );
...
```



# <a name="apidoc.module.uglify-js.DefaultsError"></a>[module uglify-js.DefaultsError](#apidoc.module.uglify-js.DefaultsError)

#### <a name="apidoc.element.uglify-js.DefaultsError.DefaultsError"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>DefaultsError (msg, defs)](#apidoc.element.uglify-js.DefaultsError.DefaultsError)
- description and source-code
```javascript
function DefaultsError(msg, defs) {
    this.message = msg;
    this.defs = defs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.DefaultsError.croak"></a>[function <span class="apidocSignatureSpan">uglify-js.DefaultsError.</span>croak (msg, defs)](#apidoc.element.uglify-js.DefaultsError.croak)
- description and source-code
```javascript
croak = function (msg, defs) {
    throw new DefaultsError(msg, defs);
}
```
- example usage
```shell
...
};

function defaults(args, defs, croak) {
    if (args === true)
        args = {};
    var ret = args || {};
    if (croak) for (var i in ret) if (HOP(ret, i) && !HOP(defs, i))
        DefaultsError.croak("'" + i + "' is not a supported option", defs);
    for (var i in defs) if (HOP(defs, i)) {
        ret[i] = (args && HOP(args, i)) ? args[i] : defs[i];
    }
    return ret;
};

function merge(obj, ext) {
...
```



# <a name="apidoc.module.uglify-js.DefaultsError.prototype"></a>[module uglify-js.DefaultsError.prototype](#apidoc.module.uglify-js.DefaultsError.prototype)

#### <a name="apidoc.element.uglify-js.DefaultsError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">uglify-js.DefaultsError.prototype.</span>constructor (msg, defs)](#apidoc.element.uglify-js.DefaultsError.prototype.constructor)
- description and source-code
```javascript
function DefaultsError(msg, defs) {
    this.message = msg;
    this.defs = defs;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.Dictionary"></a>[module uglify-js.Dictionary](#apidoc.module.uglify-js.Dictionary)

#### <a name="apidoc.element.uglify-js.Dictionary.Dictionary"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>Dictionary ()](#apidoc.element.uglify-js.Dictionary.Dictionary)
- description and source-code
```javascript
function Dictionary() {
    this._values = Object.create(null);
    this._size = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Dictionary.fromObject"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.</span>fromObject (obj)](#apidoc.element.uglify-js.Dictionary.fromObject)
- description and source-code
```javascript
fromObject = function (obj) {
    var dict = new Dictionary();
    dict._size = merge(dict._values, obj);
    return dict;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.Dictionary.prototype"></a>[module uglify-js.Dictionary.prototype](#apidoc.module.uglify-js.Dictionary.prototype)

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.add"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>add (key, val)](#apidoc.element.uglify-js.Dictionary.prototype.add)
- description and source-code
```javascript
add = function (key, val) {
    if (this.has(key)) {
        this.get(key).push(val);
    } else {
        this.set(key, [ val ]);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.del"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>del (key)](#apidoc.element.uglify-js.Dictionary.prototype.del)
- description and source-code
```javascript
del = function (key) {
    if (this.has(key)) {
        --this._size;
        delete this._values["$" + key];
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.each"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>each (f)](#apidoc.element.uglify-js.Dictionary.prototype.each)
- description and source-code
```javascript
each = function (f) {
    for (var i in this._values)
        f(this._values[i], i.substr(1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.get"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>get (key)](#apidoc.element.uglify-js.Dictionary.prototype.get)
- description and source-code
```javascript
get = function (key) { return this._values["$" + key] }
```
- example usage
```shell
...
    }

    function mangle(name) {
        if (!should_mangle(name)) {
            return name;
        }

        var mangled = cache.props.get(name);
        if (!mangled) {
            if (debug) {
// debug mode: use a prefix and suffix to preserve readability, e.g. o.foo -> o._$foo$NNN_.
var debug_mangled = "_$" + name + "$" + debug_name_suffix + "_";

if (can_mangle(debug_mangled) && !(ignore_quoted && debug_mangled in ignored)) {
    mangled = debug_mangled;
...
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.has"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>has (key)](#apidoc.element.uglify-js.Dictionary.prototype.has)
- description and source-code
```javascript
has = function (key) { return ("$" + key) in this._values }
```
- example usage
```shell
...
// only function declarations after this line

function can_mangle(name) {
    if (!is_identifier(name)) return false;
    if (unmangleable.indexOf(name) >= 0) return false;
    if (reserved.indexOf(name) >= 0) return false;
    if (options.only_cache) {
        return cache.props.has(name);
    }
    if (/^[0-9.]+$/.test(name)) return false;
    return true;
}

function should_mangle(name) {
    if (ignore_quoted && name in ignored) return false;
...
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.map"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>map (f)](#apidoc.element.uglify-js.Dictionary.prototype.map)
- description and source-code
```javascript
map = function (f) {
    var ret = [];
    for (var i in this._values)
        ret.push(f(this._values[i], i.substr(1)));
    return ret;
}
```
- example usage
```shell
...

function find_builtins() {
var a = [];
[ Object, Array, Function, Number,
  String, Boolean, Error, Math,
  Date, RegExp
].forEach(function(ctor){
    Object.getOwnPropertyNames(ctor).map(add);
    if (ctor.prototype) {
        Object.getOwnPropertyNames(ctor.prototype).map(add);
    }
});
function add(name) {
    push_uniq(a, name);
}
...
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.set"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>set (key, val)](#apidoc.element.uglify-js.Dictionary.prototype.set)
- description and source-code
```javascript
set = function (key, val) {
    if (!this.has(key)) ++this._size;
    this._values["$" + key] = val;
    return this;
}
```
- example usage
```shell
...
            // (filled with quoted properties when ignore_quoted set). Make sure we add this
            // check so we don't collide with a quoted name.
            do {
                mangled = base54(++cache.cname);
            } while (!can_mangle(mangled) || (ignore_quoted && mangled in ignored));
        }

        cache.props.set(name, mangled);
    }
    return mangled;
}

function addStrings(node, ignore) {
    var out = {};
    try {
...
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.size"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>size ()](#apidoc.element.uglify-js.Dictionary.prototype.size)
- description and source-code
```javascript
size = function () {
    return this._size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.Dictionary.prototype.toObject"></a>[function <span class="apidocSignatureSpan">uglify-js.Dictionary.prototype.</span>toObject ()](#apidoc.element.uglify-js.Dictionary.prototype.toObject)
- description and source-code
```javascript
toObject = function () { return this._values }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.JS_Parse_Error"></a>[module uglify-js.JS_Parse_Error](#apidoc.module.uglify-js.JS_Parse_Error)

#### <a name="apidoc.element.uglify-js.JS_Parse_Error.JS_Parse_Error"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglify-js.JS_Parse_Error.JS_Parse_Error)
- description and source-code
```javascript
function JS_Parse_Error(message, filename, line, col, pos) {
    this.message = message;
    this.filename = filename;
    this.line = line;
    this.col = col;
    this.pos = pos;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.JS_Parse_Error.prototype"></a>[module uglify-js.JS_Parse_Error.prototype](#apidoc.module.uglify-js.JS_Parse_Error.prototype)

#### <a name="apidoc.element.uglify-js.JS_Parse_Error.prototype.constructor"></a>[function <span class="apidocSignatureSpan">uglify-js.JS_Parse_Error.prototype.</span>constructor (message, filename, line, col, pos)](#apidoc.element.uglify-js.JS_Parse_Error.prototype.constructor)
- description and source-code
```javascript
function JS_Parse_Error(message, filename, line, col, pos) {
    this.message = message;
    this.filename = filename;
    this.line = line;
    this.col = col;
    this.pos = pos;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.MAP"></a>[module uglify-js.MAP](#apidoc.module.uglify-js.MAP)

#### <a name="apidoc.element.uglify-js.MAP.MAP"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>MAP (a, f, backwards)](#apidoc.element.uglify-js.MAP.MAP)
- description and source-code
```javascript
function MAP(a, f, backwards) {
    var ret = [], top = [], i;
    function doit() {
        var val = f(a[i], i);
        var is_last = val instanceof Last;
        if (is_last) val = val.v;
        if (val instanceof AtTop) {
            val = val.v;
            if (val instanceof Splice) {
                top.push.apply(top, backwards ? val.v.slice().reverse() : val.v);
            } else {
                top.push(val);
            }
        }
        else if (val !== skip) {
            if (val instanceof Splice) {
                ret.push.apply(ret, backwards ? val.v.slice().reverse() : val.v);
            } else {
                ret.push(val);
            }
        }
        return is_last;
    };
    if (a instanceof Array) {
        if (backwards) {
            for (i = a.length; --i >= 0;) if (doit()) break;
            ret.reverse();
            top.reverse();
        } else {
            for (i = 0; i < a.length; ++i) if (doit()) break;
        }
    }
    else {
        for (i in a) if (HOP(a, i)) if (doit()) break;
    }
    return top.concat(ret);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.MAP.at_top"></a>[function <span class="apidocSignatureSpan">uglify-js.MAP.</span>at_top (val)](#apidoc.element.uglify-js.MAP.at_top)
- description and source-code
```javascript
at_top = function (val) { return new AtTop(val) }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.MAP.last"></a>[function <span class="apidocSignatureSpan">uglify-js.MAP.</span>last (val)](#apidoc.element.uglify-js.MAP.last)
- description and source-code
```javascript
last = function (val) { return new Last(val) }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.MAP.splice"></a>[function <span class="apidocSignatureSpan">uglify-js.MAP.</span>splice (val)](#apidoc.element.uglify-js.MAP.splice)
- description and source-code
```javascript
splice = function (val) { return new Splice(val) }
```
- example usage
```shell
...
return text.replace(/\{(.+?)\}/g, function(str, p){
    return props && props[p];
});
};

function remove(array, el) {
for (var i = array.length; --i >= 0;) {
    if (array[i] === el) array.splice(i, 1);
}
};

function mergeSort(array, cmp) {
if (array.length < 2) return array.slice();
function merge(a, b) {
    var r = [], ai = 0, bi = 0, i = 0;
...
```



# <a name="apidoc.module.uglify-js.SymbolDef"></a>[module uglify-js.SymbolDef](#apidoc.module.uglify-js.SymbolDef)

#### <a name="apidoc.element.uglify-js.SymbolDef.SymbolDef"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglify-js.SymbolDef.SymbolDef)
- description and source-code
```javascript
function SymbolDef(scope, index, orig) {
    this.name = orig.name;
    this.orig = [ orig ];
    this.scope = scope;
    this.references = [];
    this.global = false;
    this.mangled_name = null;
    this.undeclared = false;
    this.index = index;
    this.id = SymbolDef.next_id++;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.SymbolDef.prototype"></a>[module uglify-js.SymbolDef.prototype](#apidoc.module.uglify-js.SymbolDef.prototype)

#### <a name="apidoc.element.uglify-js.SymbolDef.prototype.mangle"></a>[function <span class="apidocSignatureSpan">uglify-js.SymbolDef.prototype.</span>mangle (options)](#apidoc.element.uglify-js.SymbolDef.prototype.mangle)
- description and source-code
```javascript
mangle = function (options) {
    var cache = options.cache && options.cache.props;
    if (this.global && cache && cache.has(this.name)) {
        this.mangled_name = cache.get(this.name);
    }
    else if (!this.mangled_name && !this.unmangleable(options)) {
        var s = this.scope;
        if (!options.screw_ie8 && this.orig[0] instanceof AST_SymbolLambda)
            s = s.parent_scope;
        this.mangled_name = s.next_mangled(options, this);
        if (this.global && cache) {
            cache.set(this.name, this.mangled_name);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.SymbolDef.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglify-js.SymbolDef.prototype.</span>unmangleable (options)](#apidoc.element.uglify-js.SymbolDef.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (options) {
    if (!options) options = {};

    return (this.global && !options.toplevel)
        || this.undeclared
        || (!options.eval && (this.scope.uses_eval || this.scope.uses_with))
        || (options.keep_fnames
            && (this.orig[0] instanceof AST_SymbolLambda
                || this.orig[0] instanceof AST_SymbolDefun));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.TreeWalker"></a>[module uglify-js.TreeWalker](#apidoc.module.uglify-js.TreeWalker)

#### <a name="apidoc.element.uglify-js.TreeWalker.TreeWalker"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>TreeWalker (callback)](#apidoc.element.uglify-js.TreeWalker.TreeWalker)
- description and source-code
```javascript
function TreeWalker(callback) {
    this.visit = callback;
    this.stack = [];
    this.directives = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.TreeWalker.prototype"></a>[module uglify-js.TreeWalker.prototype](#apidoc.module.uglify-js.TreeWalker.prototype)

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype._visit"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>_visit (node, descend)](#apidoc.element.uglify-js.TreeWalker.prototype._visit)
- description and source-code
```javascript
_visit = function (node, descend) {
    this.push(node);
    var ret = this.visit(node, descend ? function(){
        descend.call(node);
    } : noop);
    if (!ret && descend) {
        descend.call(node);
    }
    this.pop(node);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.find_parent"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>find_parent (type)](#apidoc.element.uglify-js.TreeWalker.prototype.find_parent)
- description and source-code
```javascript
find_parent = function (type) {
    var stack = this.stack;
    for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof type) return x;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.has_directive"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>has_directive (type)](#apidoc.element.uglify-js.TreeWalker.prototype.has_directive)
- description and source-code
```javascript
has_directive = function (type) {
    var dir = this.directives[type];
    if (dir) return dir;
    var node = this.stack[this.stack.length - 1];
    if (node instanceof AST_Scope) {
        for (var i = 0; i < node.body.length; ++i) {
            var st = node.body[i];
            if (!(st instanceof AST_Directive)) break;
            if (st.value == type) return st;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.in_boolean_context"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>in_boolean_context ()](#apidoc.element.uglify-js.TreeWalker.prototype.in_boolean_context)
- description and source-code
```javascript
in_boolean_context = function () {
    var stack = this.stack;
    var i = stack.length, self = stack[--i];
    while (i > 0) {
        var p = stack[--i];
        if ((p instanceof AST_If           && p.condition === self) ||
            (p instanceof AST_Conditional  && p.condition === self) ||
            (p instanceof AST_DWLoop       && p.condition === self) ||
            (p instanceof AST_For          && p.condition === self) ||
            (p instanceof AST_UnaryPrefix  && p.operator == "!" && p.expression === self))
        {
            return true;
        }
        if (!(p instanceof AST_Binary && (p.operator == "&&" || p.operator == "||")))
            return false;
        self = p;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.loopcontrol_target"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>loopcontrol_target (label)](#apidoc.element.uglify-js.TreeWalker.prototype.loopcontrol_target)
- description and source-code
```javascript
loopcontrol_target = function (label) {
    var stack = this.stack;
    if (label) for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof AST_LabeledStatement && x.label.name == label.name) {
            return x.body;
        }
    } else for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof AST_Switch || x instanceof AST_IterationStatement)
            return x;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.parent"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>parent (n)](#apidoc.element.uglify-js.TreeWalker.prototype.parent)
- description and source-code
```javascript
parent = function (n) {
    return this.stack[this.stack.length - 2 - (n || 0)];
}
```
- example usage
```shell
...
return Object.prototype.hasOwnProperty.call(obj, prop);
}

// return true if the node at the top of the stack (that means the
// innermost node in the current output) is lexically the first in
// a statement.
function first_in_statement(stack) {
var node = stack.parent(-1);
for (var i = 0, p; p = stack.parent(i); i++) {
    if (p instanceof AST_Statement && p.body === node)
        return true;
    if ((p instanceof AST_Seq           && p.car === node        ) ||
        (p instanceof AST_Call          && p.expression === node && !(p instanceof AST_New) ) ||
        (p instanceof AST_Dot           && p.expression === node ) ||
        (p instanceof AST_Sub           && p.expression === node ) ||
...
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.pop"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>pop (node)](#apidoc.element.uglify-js.TreeWalker.prototype.pop)
- description and source-code
```javascript
pop = function (node) {
    this.stack.pop();
    if (node instanceof AST_Lambda) {
        this.directives = Object.getPrototypeOf(this.directives);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.push"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>push (node)](#apidoc.element.uglify-js.TreeWalker.prototype.push)
- description and source-code
```javascript
push = function (node) {
    if (node instanceof AST_Lambda) {
        this.directives = Object.create(this.directives);
    } else if (node instanceof AST_Directive && !this.directives[node.value]) {
        this.directives[node.value] = node;
    }
    this.stack.push(node);
}
```
- example usage
```shell
...
var is_last = val instanceof Last;
if (is_last) val = val.v;
if (val instanceof AtTop) {
    val = val.v;
    if (val instanceof Splice) {
        top.push.apply(top, backwards ? val.v.slice().reverse() : val.v);
    } else {
        top.push(val);
    }
}
else if (val !== skip) {
    if (val instanceof Splice) {
        ret.push.apply(ret, backwards ? val.v.slice().reverse() : val.v);
    } else {
        ret.push(val);
...
```

#### <a name="apidoc.element.uglify-js.TreeWalker.prototype.self"></a>[function <span class="apidocSignatureSpan">uglify-js.TreeWalker.prototype.</span>self ()](#apidoc.element.uglify-js.TreeWalker.prototype.self)
- description and source-code
```javascript
self = function () {
    return this.stack[this.stack.length - 1];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglify-js.base54"></a>[module uglify-js.base54](#apidoc.module.uglify-js.base54)

#### <a name="apidoc.element.uglify-js.base54.base54"></a>[function <span class="apidocSignatureSpan">uglify-js.</span>base54 (num)](#apidoc.element.uglify-js.base54.base54)
- description and source-code
```javascript
function base54(num) {
    var ret = "", base = 54;
    num++;
    do {
        num--;
        ret += String.fromCharCode(chars[num % base]);
        num = Math.floor(num / base);
        base = 64;
    } while (num > 0);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.base54.consider"></a>[function <span class="apidocSignatureSpan">uglify-js.base54.</span>consider (str)](#apidoc.element.uglify-js.base54.consider)
- description and source-code
```javascript
consider = function (str){
    for (var i = str.length; --i >= 0;) {
        var code = str.charCodeAt(i);
        if (code in frequency) ++frequency[code];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.base54.freq"></a>[function <span class="apidocSignatureSpan">uglify-js.base54.</span>freq ()](#apidoc.element.uglify-js.base54.freq)
- description and source-code
```javascript
freq = function (){ return frequency }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.base54.get"></a>[function <span class="apidocSignatureSpan">uglify-js.base54.</span>get ()](#apidoc.element.uglify-js.base54.get)
- description and source-code
```javascript
get = function (){ return chars }
```
- example usage
```shell
...
    }

    function mangle(name) {
        if (!should_mangle(name)) {
            return name;
        }

        var mangled = cache.props.get(name);
        if (!mangled) {
            if (debug) {
// debug mode: use a prefix and suffix to preserve readability, e.g. o.foo -> o._$foo$NNN_.
var debug_mangled = "_$" + name + "$" + debug_name_suffix + "_";

if (can_mangle(debug_mangled) && !(ignore_quoted && debug_mangled in ignored)) {
    mangled = debug_mangled;
...
```

#### <a name="apidoc.element.uglify-js.base54.reset"></a>[function <span class="apidocSignatureSpan">uglify-js.base54.</span>reset ()](#apidoc.element.uglify-js.base54.reset)
- description and source-code
```javascript
function reset() {
    frequency = Object.create(null);
    chars = string.split("").map(function(ch){ return ch.charCodeAt(0) });
    chars.forEach(function(ch){ frequency[ch] = 0 });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglify-js.base54.sort"></a>[function <span class="apidocSignatureSpan">uglify-js.base54.</span>sort ()](#apidoc.element.uglify-js.base54.sort)
- description and source-code
```javascript
sort = function () {
    chars = mergeSort(chars, function(a, b){
        if (is_digit(a) && !is_digit(b)) return 1;
        if (is_digit(b) && !is_digit(a)) return -1;
        return frequency[b] - frequency[a];
    });
}
```
- example usage
```shell
...
    f += "switch(str){";
    for (var i = 0; i < arr.length; ++i) f += "case " + quote(arr[i]) + ":";
    f += "return true}return false;";
}
// When there are more than three length categories, an outer
// switch first dispatches on the lengths, to save on comparisons.
if (cats.length > 3) {
    cats.sort(function(a, b) {return b.length - a.length;});
    f += "switch(str.length){";
    for (var i = 0; i < cats.length; ++i) {
        var cat = cats[i];
        f += "case " + cat[0].length + ":";
        compareTo(cat);
    }
    f += "}";
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
