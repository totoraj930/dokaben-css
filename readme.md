# ドカベンCSS

ドカベンのタイトル風なアニメーションをさせるCSS

[Demo](https://totoraj930.github.io/dokaben-css)

[Download](https://github.com/totoraj930/dokaben-css/archive/master.zip)

## 使い方

下記のファイルを読み込んでください。

* dokaben.css

```html
<link rel="stylesheet" href="dokaben.css">
```


### 使用例

#### 基本
```html
<p class="dokaben dkbn-loop">これはテストです</p>
```

#### 一部だけ
```html
<p>文章の中の<span class="dokaben dkbn-loop">ここだけ</span>がアニメーションされます。</p>
```

#### コマ落とし？
```html
<p>
	<span class="dokaben dkbn-loop dkbn-steps dkbn-text">コマオトシ アリ</span>
	と
	<span class="dokaben dkbn-loop dkbn-text">コマオトシ　ナシ</span>
</p>
```

#### ホバーしたとき
```html
<p><a href="#" class="dkbn-hover"><span class="dokaben dkbn-loop2">ここにマウスがのると動くよ</span></a></p>
```

#### ドカベンっぽい文字
```html
<p class="dkbn-text" style="font-size: 2em;">ドカベン</p>
```


### 高度な使い方

#### 速度を変える
```html
<p class="dokaben dkbn-loop dkbn-text" style="animation-duration: 1000ms; font-size: 2em;">ハヤイ ヤツ</p>
```

#### コマ落としを調整する
```html
<p class="dokaben dkbn-loop dkbn-text" style="animation-timing-function: steps(10); font-size: 2em;">カクカク</p>
```

### 各classの説明

|class|説明|
|-----|-----|
|`.dokaben`|アニメーションさせたい要素につける|
|`.dkbn-up`|起き上がるアニメーション|
|`.dkbn-down`|倒れるアニメーション|
|`.dkbn-loop`|up → down → up...の繰り返し|
|`.dkbn-loop2`|down → up → down...の繰り返し|
|`.dkbn-down-no`|倒れた状態にする|
|`.dkbn-steps`|アニメーションがコマ落ち(18コマ/1アニメーション)になる|
|`.dkbn-hover`|これを付けた要素がホバーされたときに子要素の`.dokaben`がアニメーションを開始する|
|`.dkbn-text`|ドカベンっぽい文字にする|


### 注意

`.dokaben`を指定した要素は`display: inline-block`になります。
デザインが崩れる原因となりますので入れ子にするなどして対処してください。

## 著者
**Reona Oshima (totoraj)**
* [http://totoraj.net](http://totoraj.net/)
* [Twitter: @totoraj930](https://twitter.com/totoraj930/)


## ライセンス
Copyright &copy; 2016 Reona Oshima (totoraj)  
This work is released  under the MIT License.  
<http://opensource.org/licenses/mit-license.php>