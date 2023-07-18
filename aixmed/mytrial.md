## trial

``` mermaid
erDiagram
    IMG_META ||--o{ STORAGE : save
    IMG_META {
        string imageID PK, FK
        string scanner "scanner model"
        float mpp "micron per pixel"
        string iccProfile
        int width
        int height
        int wsifsize "filesize (KB)"
        int bestZ "best focal layer"
        int Zstack "muliple layers"
    }
    IMG_META ||--o{ INFERENCE : inference
    INFERENCE {
        string decartVersion PK
        string modelVersion
        string envOS
        string envCPU
        string envGPU
        string actDate
        int sCells
        int aCells
        int inferenceLayer
        string cnvTime "consumed time for conversion"
        string aixTime "consumed time for inference"
        string dc2Time "conversion+inference time"
    }
    STORAGE {
        string wsiPath
        string medPath
        string aixPath
    }
    WSI only one to zero or more IMG_META : has_own
```
