# <a name="call-microsoft-graph-from-a-cloud-solution-provider-application"></a>クラウド ソリューション プロバイダーのアプリケーションからの Microsoft Graph の呼び出し

> **注:**このトピックは Microsoft クラウド ソリューション プロバイダー (CSP) アプリケーション開発者**のみ**に適用されます。[Microsoft クラウド ソリューション プロバイダー (CSP)](https://partner.microsoft.com/en-US/cloud-solution-provider) プログラムは、マイクロソフトパートナーが Microsoft Online サービスを再販し、管理することを可能とします。

このトピックは、パートナーが管理する顧客のアプリケーションへのアクセスを Microsoft Graph を介し、[認証コードの許可のフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-code)または[サービス間クライアント資格情報フロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)により許容する方法を説明します。

**重要:**CSP アプリケーションからの Microsoft Graph の呼び出しは、ディレクトリ リソース (**user**、**group**、**device**、**organization** など) と [Intune](..\api-reference\beta\resources\intune_graph_overview.md) リソースでのみサポートされています。

## <a name="what-is-a-partner-managed-application"></a>パートナー管理アプリケーションとは

CSP プログラムは、マイクロソフトパートナーが Microsoft Online サービス (Office 365、Microsoft Azure、CRM Online など) を再販し、管理することを可能とします。顧客サービスの管理は、特に任命されたパートナー ユーザー (エージェントといいます) にその顧客の環境をアクセスし、設定する権限を与える Delegated Admin 権限により行います。

さらに、パートナー開発者は顧客の Microsoft サービスを管理する**パートナー管理アプリケーション**を作成できます。すべての顧客は自動的にパートナー管理アプリケーションを事前承認するため、パートナー管理アプリケーションは*事前承認*アプリケーションとも呼ばれます。つまり、顧客テナントのユーザーがパートナー管理アプリケーションを使用するには、同意のプロンプトは不要です。パートナー管理アプリケーションは Delegated Admin 権限を継承するため、パートナーエージェントもパートナー管理アプリケーションを介して顧客にアクセスする権限を持ちます。

## <a name="how-to-set-up-a-partner-managed-application"></a>パートナー管理アプリケーションのセットアップ方法

顧客のデータをアクセスする特権が付与された場合、アプリケーションは*パートナー管理*と表示されます。

> **注:**パートナー管理アプリケーションはパートナーテナントに*のみ*設定でき、顧客テナントのリソースを管理するため、パートナー管理アプリケーションは**マルチ テナント アプリケーション**として**設定しなければなりません**。

### <a name="register-and-configure-a-multi-tenant-app"></a>マルチ テナント アプリケーションの登録と構成

ここで必要な最初の手順は、他のマルチテナントのアプリケーションの登録と設定の手順とほぼ同じです。

1. [Azure ポータル](https://portal.azure.com)を使い、パートナー テナントに[アプリケーションを登録します](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-app-registration)。パートナー管理アプリケーションとして機能するよう、アプリケーションを [multi-tenant app](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant) として設定します。また、アプリが複数の地域で配布、販売される場合は、<a href="#region">ここ</a>で示すようにそれぞれの地域で登録する必要があります。
2. 再度 Azure ポータルから、最小限の特権のアプローチにより*必要となる権限*でマルチテナントのアプリケーションを設定します。

### <a name="pre-consent-your-app-for-all-your-customers"></a>アプリをすべての顧客について事前同意します。

最後に、パートナー管理アプリケーションに設定した権限をすべての顧客に付与します。そのためには、Azure AD powershell V2 を使用して、アプリを示す **servicePrincipal** をパートナー テナントの *Adminagents* グループに追加します。Azure AD PowerShell V2 は、[ここ](https://www.powershellgallery.com/packages/AzureAD)からダウンロードし、インストールできます。*Adminagents* グループと **servicePrincipal** を検索し、これをグループに追加するには以下の手順に従います。

1. PowerShell セッションを開き、サインイン ウィンドウに、管理者資格情報を入力してパートナーのテナントに接続します。

    ```PowerShell
    Connect-AzureAd
    ```

2. *Adminagents* を表すグループを探します。

    ```PowerShell
    $group = Get-AzureADGroup -Filter "displayName eq 'Adminagents'"
    ```

3. 使用しているアプリケーションと同じ *appId* を持つサービス プリンシパルを検索します。

    ```PowerShell
    $sp = Get-AzureADServicePrincipal -Filter "appId eq '{yourAppsAppId}'"
    ```

4. 最後に、サービス プリンシパルを *Adminagents* グループに追加します。

    ```PowerShell
    Add-AzureADGroupMember -ObjectId $group.ObjectId -RefObjectId $sp.ObjectId
    ```

## <a name="token-acquisition-flows"></a>トークン取得のフロー

パートナー管理アプリケーションのトークン取得フロー、つまり[認証コード付与のフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-code)と[サービス間クライアント資格情報のフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)は、普通のマルチテナントのアプリケーションと同じです。

すべての顧客テナントへの事前承認済みアクセス以外に、パートナー管理アプリケーションにはもうひとつの機能があります。それは、エージェントがアプリケーションを使って顧客テナントのデータへアクセスできるようにする機能です (delegated admin 権限を使って)。概念的には次のように動作します。

1. エージェントは、パートナー テナントが発行したエージェント自身のユーザー資格情報を使ってアプリケーションにサインインします。
2. アプリケーションは目的となるパートナー管理顧客テナントへのアクセス トークンを要求します。
3. アプリはアクセス トークンを使用して、Microsoft Graph を呼び出します。

これは、標準的な[認証コード付与のフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-code)ですが、エージェントがパートナーのアカウントを使用してサインインする必要がある点が異なります。わかりやすくするため、パートナーテナントを *partner.com* (エージェントのホーム テナント) とし、顧客を *customer.com* とします。

1. [認証コードを取得する](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code)アプリケーションは ```/authorize``` エンドポイントに要求を送信します。ターゲット テナントとして**顧客テナント** (この例では ```customer.com```) を指定しなくてはなりません。エージェントは、引き続き自分の ```username@partner.com``` アカウントでサインインします。

    ```http
    GET https://login.microsoftonline.com/customer.com/oauth2/authorize
    ```

2. [承認コードを使用してアクセス トークンを取得する](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token)アプリケーションは、```token``` エンドポイントに要求を送る際、ターゲット テナントを**顧客テナント** (この例では ```customer.com```) とする必要があります。

    ```http
    POST https://login.microsoftonline.com/customer.com/oauth2/token
    ```

3. トークンへのアクセスができたら、HTTP 認証ヘッダーにトークンを入れて Microsoft Graph を呼び出します。

    ```http
    GET https://graph.microsoft.com/beta/users
    Authorization: Bearer <token>
    ```

## <a name="register-your-app-in-the-regions-you-support"></a>サポートする地域でのアプリケーションの登録
<a name="region"></a>

今のところ、CSP 顧客契約は 1 つの地域に限定されています。パートナー管理アプリケーションには、いくつかの制限があります。つまり、販売を展開する地域ごとにテナントを用意する必要があります。たとえば、パートナー管理アプリケーションを米国のテナントに登録し、顧客は EU に在住している場合は、パートナー管理アプリケーションは機能しません。同一地域の顧客を管理するには、各地域パートナーのテナントは、各自の一連のパートナー管理アプリケーションを維持する必要があります。これにより、アプリケーションに顧客のサインイン名を取得し、地域専用のどのパートナー管理アプリケーションを使用するか決定するための (サインイン前の) ロジックを追加する必要が生じることがあります。

## <a name="calling-microsoft-graph-immediately-after-customer-creation"></a>顧客作成後すぐに Microsoft Graph を呼び出す

[Partner Center API](https://partnercenter.microsoft.com/en-us/partner/developer) を使用して新しい顧客を作成すると、新しい顧客テナントも作成されます。さらに、パートナーの関連付けが行われ、この新しい顧客テナントとレコードのパートナーとしての関連付けが行われます。このパートナー関係が新しい顧客テナントに反映されるには最長 3 分かかることがあります。作成後すぐにアプリケーションが直接に Microsoft Graph を呼び出すと、アクセス拒否エラーを受け取ることがあります。既存の顧客が招待を受け付けると、これと同じ遅延が発生することがあります。このため、事前承認は顧客テナントに存在しているパートナー関係に依存します。

この問題を回避するには、顧客の作成後、パートナーアプリケーションは (Microsoft Graph 呼び出しのための) トークン取得のために Azure AD を呼び出す前に **3 分間**待機することを推奨します。ほとんどの場合がこれで解決します。3 分待機しても認証エラーが発生する場合は、さらに 60 秒間待機してからもう一度お試しください。

> **注:**再試行のためには、Microsoft Graph を呼び出す前に Azure  AD から新しいアクセス トークンを取得する必要があります。既存のアクセストークンを使用して Microsoft Graph を呼び出すことはできません。アクセス トークンは 1 時間のみ有効で、事前承認の要求が含まれないためです。
