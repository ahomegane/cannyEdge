
html5 canvas で使用できる キャニーエッジアルゴリズム

demo:
http://jsdo.it/ahomegane/uCAO

画像からの線の抽出ができます。

・グレースケール変換
・ガウシアンフィルタ（ぼかし）
・ソーベルフィルタ（エッジ）
のみの処理も可能。

var ced = new cannyEdgeDetecotor({
    imageData: this.imageData,
    //以下省略可
    GaussianSiguma: 3,
    GaussianSize: 5,
    hysteresisHeigh: 100,
    hysteresisLow: 10,
    isConvertGrayScale: true,
    isApplyGaussianFilter: true,
    isApplySobelFilter: true,
    isHysteresisThreshold: true
});