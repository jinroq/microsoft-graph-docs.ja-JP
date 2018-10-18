# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Microsoft Graph のバージョン管理、サポートと重大な変更の方針 

この記事は Microsoft Graph のサポート重大な変更の方針と、現在使用可能な Microsoft Graph API のバージョンについて説明します。

## <a name="support-policy-and-deprecation-information"></a>サポート ポリシーと廃止の情報

Microsoft Graph は [Microsoft ライフサイクル ポリシー](https://support.microsoft.com/en-us/lifecycle)に従います。 

Microsoft Graph REST API と Microsoft Graph SDK の新しいバージョンがリリースされると、それ以前のバージョンは廃止されます。Microsoft は API または SDK が廃止される少なくとも 24 か月前までにそれ以前のバージョンを非推奨に指定します。 

API のメジャー バージョンを新しくする場合 (たとえば、v1.0 から v2.0 へ)、現在のバージョン (この例では v1.0) が即時に非推奨になり、この発表から 24 か月後以降、サポートが打ち切られます。 サービスのセキュリティと信頼性向上のためにこのポリシーを変更することがあります。  

API が非推奨と指定された場合、できるだけ早く最新バージョンへ移行することを強くお勧めします。 場合によっては、元のAPIが非推奨になってからすぐに、新しいアプリケーションで新しい APIの使用を開始する必要があることを、お知らせします。 そのような場合、現在非推奨 APIを使用しているアクティブなアプリケーションのみが使用し続けることができます。   

### <a name="api-contract-and-non-backward-compatible-changes"></a>API コントラクトと下位互換性のない変更

Microsoft Graph にはバージョン更新の変更履歴があります。バージョン更新に伴う変更は [Microsoft Graph Microsoft Graph の変更ログ](changelog.md)に表示されています。Microsoft Graph には新しい機能とデータが追加されたため、下位互換性のない変更が加えられた API では、バージョン番号を更新しています。 

次に、下位互換性のない変更の例を示します。

 - URL またはリソースに関する基本的な要求や応答の変更    
 - 宣言済みプロパティの型の削除、変更と、その名前の変更
 - API と API パラメーターの削除または名前の変更
 - 必須の要求ヘッダーの追加

次に、下位互換性のある変更の例を示します。

 - Null 許容型プロパティや既定値を持つプロパティの追加
 - 列挙型へのメンバーの追加
 - オープン拡張情報の削除、変更と、その名前の変更
 - 注釈の削除、変更と、その名前の変更
 - 既存のコレクションへのページングの導入
 - エラー コードの変更
 - プロパティの順序の変更
 - リソース ID のような不透明な文字列の長さまたは形式の変更

>**注:** 下位互換性のある変更の一覧は適時変更されます。独自のクライアント プロクシ (WCF クライアントなど) を作成する場合は、ガイドラインとしては Microsoft Graph API サービスにあらかじめ定義されていないプロパティや派生型をクライアント アプリケーションが受け入れることができるように準備してください。Microsoft Graph API は「[Microsoft REST API ガイドライン](https://github.com/microsoft/api-guidelines/)」の「[バージョン管理のモデル](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning)」セクションの説明に従っています。 

## <a name="versions"></a>バージョン

現在、以下のバージョンの Microsoft Graph API が使用できます。

### <a name="beta-version"></a>ベータ版
Microsoft Graph API のベータ版は、`https://graph.microsoft.com/beta`で公開されており、現在_**プレビュー段階**_ の機能が含まれています。 ベータ版 API のドキュメントは、「[Microsoft Graph ベータ エンドポイント リファレンス](../api-reference/beta/beta-overview.md)」を参照してください。 ベータ版には随時重大な変更が発生することがあります。 本番環境が /beta API に依存することのないようにしてください。

ベータ版の機能が現行バージョンに採用される保証はありません。Microsoft Graph API チームの判断でベータ版の機能が一般提供 (GA) に十分なものとなったとき、その機能が最新バージョンに追加されます。機能の採用が現行バージョンに重大な変更を招く場合は、バージョン番号が更新され、新規バージョンが現行バージョンに変わります。開発者コミュニティは、新機能や既存のベータ版 API 機能の現行バージョンでの採用希望などの機能の要望を [UserVoice](https://officespdev.uservoice.com/) に投稿できます。 

### <a name="current-version"></a>現在のバージョン

Microsoft Graph の現在のバージョンは、v1.0 です。Microsoft Graph API /v1.0 バージョンは `https://graph.microsoft.com/v1.0` で一般提供されており、一般的に利用可能で本番環境での運用準備が整った機能が含まれています。v1.0 API のドキュメントの各部は、目次から参照できます。

### <a name="deprecated-and-unsupported-versions"></a>非推奨およびサポートされないバージョン

現在、Microsoft Graph には非推奨のバージョンはありません。

## <a name="terms-of-use"></a>利用規約

Microsoft Graph API を使用すると、お客様は [利用規約](https://developer.microsoft.com/en-us/graph/docs/misc/terms-of-use) に同意したこととなります。 

お客様からのフィードバックを重視しています。[スタック オーバーフロー](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest)でご連絡いただけます。ご質問には {MicrosoftGraph} のタグを付けてください。
