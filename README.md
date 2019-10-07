### go-plus
---
https://github.com/joefitzgerald/go-plus

```js
// spec/test/tester-spec.js
import path from 'path'
import { lifecycle } from './../spec-helpers'
import { it, fit, ffit, beforeEach, runs } from '../async-spec-helpers'

describe('tester', () => {
  let tester = null
  
  beforeEach(async () => {
    lifecycle.setup()
    atom.config.set(
      'go-plus.test.converageHighlightMode',
      'covered-and-uncovered'
    )
    await lifecycle.activatePackage()
    const { mainModule } = lifecycle
    tester = mainModule.loadTester()
  })
  
  afterEach(() => {
    lifecycle.teardown()
  })
  
  describe('go test args', () => {
    beforeEach(() => {
      atom.config.unset('go-plus.config.additionaltestArgs')
    })
    
    afterEach(() => {
      atom.config.set('go-plus.test.runTestsWithShortFlag', true)
      atom.config.set('go-plus.test.runTestsWithVerboseFlag', false)
    })
    
    it('', () => {
    })
    
    it('', () => {
    })
    
    describe('', () => {
      it('', () => {
      })
      
      it('', () => {
      })
    })
  })
  
  describe('with a gopath setup', () => {
  })
  
  describe('when run tests on save is disabled', () => {
    beforeEach(() => {
      atom.config.set('go-plus.test.runTestsOnSave', false)
    })
    
    it('does not run tests automatically on save', async () => {
      spyOn(tester, 'runTests')
      await tester.handleSaveEvent(editor)
      expect(tester.runTests).not.toHaveBeenCalled()
    })
    
    it('displays coverage for go source', async () => {
      await teaster.runTests(editor)
      
      const layers = tester.markedEditors.get(editors.id)
      expect(layers).toBeTruthy()
      let layerids = layers.split(',')
      let coveredLayer = editor.getMarkerLayer(layerids[0])
      let uncoveredLayer = editor.getMarkerLayer(layerids[1])
      expect(coveredLayer).toBeTruthy()
      expect(uncoveredLayer).toBeTruthy()
      
      let coveredmarkers = coveredLayer.getMarkers()
      expect().tobeDefined()
      
    })
    
    it('', async () => {
      let 
      let
      let
      expect()
      expect()
      
      let
      expect()
      expect()
      expect()
      let range
      expect()
      expect()
      expect()
      expect()
      
      let 
      expect()
      expect()
      expect()
      rage
      expect()
      expect()
      expect()
      expect()
      expect()
      
      tester.clearMarkers(editor)
      expect()
      expect()
    })
  })
})
```

```
```

```
```


