---
title: 'Project Rome を利用したクロスデバイス アプリのビルド '
description: 'Project Rome を使用することにより、デバイスやプラットフォームをシームレスに超えて利用できるエクスペリエンスを構築できます。これにより、ユーザーのストレスが少なくなり、アプリの利用が推進されます。 アプリケーションが Project Rome API を利用して複数のデバイスやプラットフォーム間でデータを共有するには、プラットフォーム固有のアプリに関する情報を含むクロスデバイス アプリを構成する必要があります。 '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: f54f38c5d047d2b5d790e5bea48fdb27f54b4004
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987084"
---
# <a name="build-cross-device-apps-powered-by-project-rome"></a>Project Rome を利用したクロスデバイス アプリのビルド 

Project Rome を使用することにより、デバイスやプラットフォームをシームレスに超えて利用できるエクスペリエンスを構築できます。これにより、ユーザーのストレスが少なくなり、アプリの利用が推進されます。 アプリケーションが Project Rome API を利用して複数のデバイスやプラットフォーム間でデータを共有するには、プラットフォーム固有のアプリに関する情報を含むクロスデバイス アプリを構成する必要があります。 

クロスデバイス アプリでは、次のことが可能です: 

- Microsoft Graph で Project Rome のアクティビティ フィード API を利用する。  
- Project Rome SDK for Windows、Android、iOS を使用することにより、複数のプラットフォーム固有アプリケーションからなるグループによって公開されるユーザー アクティビティを読み書きする。
-  Project Rome SDK for Android または iOS を使用することによって、Project Rome のデバイス リレー機能でアプリのターゲットを切り替える。

**アクティビティ フィード API により、デバイス間を移動した際に直前の作業位置から再開する**

Windows、iOS、Android、Web 用のアプリを関連付けるようクロスデバイス アプリを構成することにより、各プラットフォームのアプリで、グループ内の任意のアプリにより公開されたユーザー アクティビティを読み書きできます。 

たとえば、あるユーザーが仕事場にある自分の PC でプレス リリースを仕上げた後、友達と夕食を食べに行ったとします。 レストランで上司から彼女に連絡があり、大至急誤字を修正するように命じられます。 彼女は、自分の Android スマートフォンでアプリを開き、先ほど編集していたプレス リリースを示すカードを表示します。 彼女は、そのカードをタップしてそれを開き、必要な修正をプレス リリースに加えた後、友達との会話に戻ります。 
 
このクロスデバイス アプリ構成を整備することにより、ユーザーのアクティビティ フィードが複数のデバイスやプラットフォームの間でとても簡単に同期されるため、ユーザーがアプリのどの面からでも、重要な作業を直前に終わったところから再開できるようなエクスペリエンスを構築できます。 

**デバイス リレー API により適切なタイミングで適切な画面を選ぶ**

アプリが利用可能なそれぞれのプラットフォームでプッシュ通知認証情報が有効になるようクロスデバイス アプリを構成することにより、プラットフォームに関係なく、アプリを使用する任意のデバイスにコマンドまたは通知が配信されるようにすることができます。 

たとえば、あるユーザーが仕事帰りのバスの中でビデオを見ているとします。 彼女が自宅に着いて、アプリをタップして Xbox One でそのビデオを起動すると、先ほどの続きを大画面で見ることができます。 

アプリが利用可能な各プラットフォームでプッシュ通知認証情報をクロスデバイス アプリに関連付けると、ユーザーのアプリがデバイス間でコマンドを送信できるようになります。これにより、リアルタイムに複数の画面の間を移動したり、別のデバイスにワークフローを移行したりするようなエクスペリエンスを構築できます。 

## <a name="select-the-right-hosting-method-for-your-cross-device-app-configuration"></a>クロスデバイス アプリ構成のための適切なホスティング方式を選択する
クロスデバイス アプリ構成は、ドメイン上の JSON ファイルとして、または [Windows デベロッパー センター](https://developer.microsoft.com/ja-JP/windows)により構成可能なプロファイルとしてホスティングできます。 ホスティング オプションは、アプリで有効にする Project Rome 機能に基づいて選択します。 

### <a name="windows-dev-center-profile-recommended"></a>Windows デベロッパー センターのプロファイル (推奨) 
Project Rome のすべて機能は、[Windows デベロッパー センター](https://developer.microsoft.com/ja-JP/windows)で管理されるクロスデバイス アプリを使用してアクセスできます。 また、Windows デベロッパー センターにより、クロスデバイス アプリ構成のあらゆる変更を管理するための*最善の*手段が提供されます。 変更内容を運用環境に公開する準備ができるまで、既存のプロファイルの更新内容を安全に保存できます。 デベロッパー センターで既存のクロスデバイス アプリの変更内容を公開すると、新しいプロファイルは、約 **1 時間**後に有効になります。  

### <a name="externally-hosted-json-file-limited"></a>外部ホスティングの JSON ファイル (制限あり) 
外部ホスティングされる JSON ファイルとして管理されるクロスデバイス アプリを使用することにより、サポートされるすべてのプラットフォーム上で、次の Project Rome 機能を使用することができます:  

* [アクティビティ フィード API](/graph/api/resources/activity-feed-api-overview?view=graph-rest-1.0) を使用してすべてのプラットフォームからユーザー アクティビティを読み書きする
* Project Rome SDK を使用してすべてのプラットフォーム (Windows、iOS、Android、web) からユーザー アクティビティを書き込む。

それらの機能に**のみ**アクセスする場合、クロスデバイス アプリ構成は、ドメイン上で JSON ファイルとして外部的にホスティングできます。

## <a name="configure-a-cross-device-app-using-the-windows-dev-center"></a>Windows デベロッパー センターを使用してクロスデバイス アプリを構成する
クロスデバイス アプリ ID は、自分の所有するドメインとして表されます。 そのドメインは、自分のドメイン上でホスティングされる JSON ファイルとして、または Windows デベロッパー センターにより構成可能なものとして保存されているプラットフォーム固有のアプリ ID のマッピングを指します。 クロスデバイス アプリ ID を表すために使用するドメインを特定したら、次に、関連するプロファイルを構成するための情報を収集する必要があります。 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id-and-enable-domain-verification"></a>手順 1: クロスデバイス アプリ ID のためのセキュリティ保護されたドメインを選択し、ドメイン検証を有効にする
クロスデバイス アプリ ID として使用されるドメインは、トップレベルのドメインかサブドメインで、TLS で保護されていなければなりません。 例: https://contoso.com または https://myapp.contoso.com。しかし、https://myapp.contoso.com/somepath は無効です。 **ドメイン (またはサブドメイン) はクロスデバイス アプリごとに固有でなければなりません。** しかし、単一のクロスデバイス アプリにどのアプリを関連付けるかは、サポートする予定のクロスプラットフォームの動作に基づいて自分で決定します。 

たとえば、一連のゲーム アプリを手がけるアプリ開発者は、アプリごとに別個のサブドメインを使い分けることにより、複数のデバイスやプラットフォームでデータを読んで再開可能なユーザー アクティビティにのみ確実に各アプリがサブスクライブされるようにするかもしれません。 一方、連携動作するよう設計された一連の生産性アプリ スイートを手がけるアプリ開発者は、そのすべてに共通の単一のドメインを使用することにより、デバイスが変わってもアプリでスイートのメンバーを立ち上げることができるようにするかもしれません。  

#### <a name="assert-domain-ownership-with-the-windows-dev-center"></a>Windows デベロッパー センターによるドメインの所有権のアサート
Windows デベロッパー センターを使用してクロスデバイス アプリの構成を管理すると、クロスデバイス アプリ ID を表すドメインはクロスデバイス アプリ プロファイルの一部として保存されるため、Microsoft はドメイン所有者を確認することができます。 クロスデバイス アプリ構成を公開するには、ドメインの所有者であることが**検証されなければなりません**。そのため、最初にこれに取り組むのは良いことです。ドメインがまだ検証されていない場合、クロスデバイス アプリの詳細を保存し、この手順の完了後に再度検証を実行することにより、クロスデバイス アプリを公開できるようになります。

クロスデバイス アプリのドメイン所有権を主張するには、デベロッパー センターで提供される固有の値を使って、そのドメインに対応する [DNS TXT](https://go.microsoft.com/fwlink/?linkid=871417) エントリを追加する必要があります。 この値は、クロスデバイス アプリごとに固有です。 アプリのための固有の値を調べるには、Windows デベロッパー センターにサインインし、左側のメニューから **[クロスデバイス エクスペリエンス]** を選択して、新しいクロスデバイス アプリの構成を開始します。 新しいクロスデバイス アプリに名前を付けた後、サブメニューから **[クロスデバイス アプリのドメインを検証する]** を選択します。 このページには、固有の値が **インラインで**表示された手順が示されます (例: MS=95ff4557-813f-45a5-b2f6-1f94170b979f)。 'MS=' の部分も含めた値全体をコピーしてください。

### <a name="step-2-collect-your-platform-specific-application-ids"></a>手順 2: プラットフォーム固有のアプリケーション ID を収集する
[Project Rome API](/graph/api/resources/project-rome-overview?view=graph-rest-1.0) を使用する、各アプリケーションおよびプラットフォームのプラットフォーム固有アプリケーション ID を収集します。

クロスデバイス アプリ ID に関連付けるため、それぞれのプラットフォーム固有のアプリケーション ID を収集する必要があります。 Windows デベロッパー センターを使用すると、デベロッパー アカウントに関連するユニバーサル Windows プラットフォーム アプリの中から選択することができます。しかし、win32、iOS、Android のアプリについては、アプリケーション ID を手動で指定し、関連する Web アプリの主要 URL を特定する必要があります。 プラットフォームごとに最大 10 個の ID を関連付けることができます。 

ID を検索するには:

* **windows_universal** - UWP アプリごとに 1 つの AUMID を提供します。 詳細については、「[インストール済みアプリのアプリケーション ユーザー モデル ID を検索する (Industry 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82))」および「[アプリケーション](https://docs.microsoft.com/ja-JP/uwp/schemas/appxpackage/appxmanifestschema/element-application)」を参照してください。
* **windows_win32** - アプリごとに 1 つの AUMID を提供します。 win32 アプリの場合、この情報を取得するにはスクリプトを使用する必要があります。 詳細については、「[インストール済みアプリのアプリケーション ユーザー モデル ID を検索する (Industry 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82))」を参照してください。
* **android** - 詳細については、「[パッケージ名の変更](https://developer.android.com/studio/build/application-id.html#change_the_package_name)」を参照してください。 
* **ios** - 詳細については、「[バンドル](https://developer.apple.com/documentation/foundation/bundle)」および「[必須プロパティ、ローカライズ可能なプロパティ、編集可能なプロパティ](https://help.apple.com/itunes-connect/developer/#/devfc3066644)」を参照してください。
* **msa** – [アプリケーション登録ポータル](https://apps.dev.microsoft.com)にサインインします。 自分の任意のアプリについて、アプリ ID/クライアント ID を確認できます。 Live SDK (16 進値) と統合アプリ ID (GUID) の両方がサポートされています。   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>手順 3: Microsoft アカウントまたは Azure AD のサポートを構成する
クロスデバイス エクスペリエンスを有効にするには、アプリ ユーザーが  [Microsoft アカウント](https://account.microsoft.com/account) または  [Azure Active Directory](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-developers-guide)  (Azure AD) アカウントのいずれかでサインインする必要があります。 クロスデバイス アプリ構成の一部として認証をサポートするためのアプリ ID/クライアント ID を提供することにより、クロスプラットフォーム サポートが有効になります。 最大 10 個のインスタンスを提供できます。

既存のアプリ ID/クライアント ID を検索するか、またはデベロッパー カウントで[アプリケーション登録ポータル](https://apps.dev.microsoft.com)にサインインすることにより新しい ID をプロビジョニングします。 そのポータルにサインインすると、自分の任意のアプリのアプリ ID/クライアント ID を確認できます。 Live SDK (16 進値) と統合アプリ ID (GUID) の両方がサポートされています。   

Azure AD のユーザーをサポートするアプリケーションをビルドする場合、[アプリケーション登録ポータル](https://apps.dev.microsoft.com)により発行される統合アプリケーション ID を使用していないなら、Azure アプリのアプリケーション ID のための GUID を提供することが必要になります。 テナントの GUID を調べるには: 

1. [Azure portal](https://portal.azure.com)にサインインします。 
2. **Azure Active Directory** を選択します。
3. **[管理]** の下で **[アプリの登録]** を選択します。 
4. リストからアプリを選択すると、**[基本]** の下にアプリケーション ID (GUID) が表示されます。

### <a name="step-4-configure-support-for-cross-platform-push-notifications-optional"></a>手順 4: クロスプラットフォーム プッシュ通知のサポートを構成する (オプション) 
クロスデバイス アプリを Windows デベロッパー センターで構成することにした場合は、Android および iOS プッシュ メッセージング プラットフォーム用の API で使用する認証情報を提供することにより、クロスプラットフォーム プッシュ通知のサポートを有効にすることができます。 それらは、Project Rome SDK for iOS および Android を使用していて、ユーザー アクティビティの公開以外のことをする場合に必須です。 Project Rome API for Microsoft Graph のみを使用する場合は、この手順を実行する必要はありません。 プラットフォームごとに認証情報を最大 10 セット関連付けることができます。 

>**重要:** プッシュ通知認証情報は、外部ホスティング JSON ファイルには保存しないでください。

ID を検索するには:

* 
  **Windows 通知サービス** - 「[アプリの登録とクラウド サービスのための認証情報の受け取り](https://docs.microsoft.com/en-us/previous-versions/windows/apps/hh913756(v=win.10)#registering-your-app-and-receiving-the-credentials-for-your-cloud-service)」および「[アプリケーション登録ポータル](https://apps.dev.microsoft.com)」を参照してください。
* **Apple Push Notification Service** -「[APN の概要](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/APNSOverview.html)」を参照してください。
* **Google Cloud Messaging** - 「[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)」を参照してください。

**注:** Firebase を使用することにより iOS デバイスに Android 認証情報を使用して通知をプッシュしている場合は、クロスデバイス アプリ構成の一部として APN 認証情報を提供する必要があります。 

## <a name="configure-a-cross-device-app-using-an-externally-hosted-json-file"></a>外部ホスティング JSON ファイルを使用してクロスデバイス アプリを構成する
クロスデバイス アプリ ID は、自分の所有するドメインとして表されます。 そのドメインは、自分のドメイン上でホスティングされる JSON ファイルとして、または Windows デベロッパー センターにより構成可能なものとして保存されているプラットフォーム固有のアプリ ID のマッピングを指します。 クロスデバイス アプリ ID を表すために使用するドメインを特定したら、次に、関連するプロファイルを構成するための情報を収集する必要があります。 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id"></a>手順 1: クロスデバイス アプリ ID のためのセキュリティ保護ドメインを選択する
クロスデバイス アプリ ID は、自分の所有するドメインとして表されます。 これは、トップレベルのドメインかサブドメインのいずれかで、TLS で保護されていなければなりません。 例: https://contoso.com または https://myapp.contoso.com。しかし、https://myapp.contoso.com/somepath は無効です。 ドメイン (またはサブドメイン) はクロスデバイス アプリごとに固有でなければなりません。 しかし、単一のクロスデバイス アプリにどのアプリを関連付けるかは、サポートする予定のクロスプラットフォームの動作に基づいて自分で決定します。 

たとえば、一連のゲーム アプリを手がけるアプリ開発者は、アプリごとに別個のサブドメインを使い分けることにより、複数のデバイスやプラットフォームでデータを読んで再開可能なユーザー アクティビティにのみ確実に各アプリがサブスクライブされるようにするかもしれません。 連携動作するよう設計された一連の生産性アプリ スイートを手がけるアプリ開発者は、そのすべてに共通の単一のドメインを使用することにより、デバイスが変わってもアプリでスイートのメンバーを立ち上げることができるようにするかもしれません。  

#### <a name="assert-domain-ownership-with-an-externally-hosted-json-file"></a>外部ホスティング JSON ファイルによるドメイン所有権のアサート 
外部ホスティング JSON ファイルを使用してクロスデバイス アプリを管理している場合は、cross-platform-app-identifiers ファイルの中に Microsoft アカウントまたは Azure AD アプリ ID を含めることにより、ドメイン所有権をアサートします。 ドメイン所有権は、アクティビティ フィード API を使用してユーザー アクティビティを作成する際に、公開プロセスの一部として検証されます。

ドメイン上で頻繁にリクエストが生成されるのを回避するため、JSON ファイルの内容はシステムによりキャッシュに入れられます。 構成されている場合、キャッシュ更新のタイミングを評価する際に、サービスにより HTTP キャッシュ ヘッダーが考慮されます。 構成されていない場合、サービスは 24 時間ごとに更新されます。 

### <a name="step-2-collect-your-platform-specific-application-ids-and-construct-your-json-file"></a>手順 2: プラットフォーム固有アプリケーション ID を収集し、JSON ファイルを構成する
アクティビティ フィードやデバイス リレー API を使用するアプリケーションとプラットフォームのそれぞれについて、プラットフォーム固有のアプリケーション ID を収集します。 

クロスデバイス アプリ ID に関連付けるため、それぞれのプラットフォーム固有のアプリケーション ID を収集する必要があります。 外部ホスティング JSON ファイルを使用する場合、クロスデバイス アプリの一部として構成するプラットフォーム固有アプリのそれぞれについてアプリ ID を収集し、それらをアセンブルして指定された形式にする必要があります。 プラットフォームごとに最大 10 個の ID を関連付けることができます。 

#### <a name="constructing-your-cross-platform-app-identifiers-file"></a>cross-platform-app-identifiers ファイルの構成
JSON ファイル自体の名前は **cross-platform-app-identifiers** でなければならず、HTTPS ドメインのルートでホスティングされていなければなりません。 ファイルの内容は、アプリケーションでサポートされるプラットフォームと、それらのプラットフォーム上のアプリケーション ID とのマッピングの JSON 配列です。 このファイルを構成する際には、Project Rome API を使用するアプリケーションおよびプラットフォームのそれぞれについて、JSON オブジェクトを 1 つずつ含めます。 
 
このファイルにより、同じプラットフォーム ID で複数の JSON オブジェクトが可能になります。 たとえば、iPhone アプリと iPad アプリは、それぞれ iOS をプラットフォーム値として、別個の JSON オブジェクトとして列挙される必要があります。 次の例に、Web プラットフォーム ID を示します。
 
すべてのプラットフォームについて JSON オブジェクトを含める必要はありません。 アプリケーションが Project Rome API を使用するプラットフォームについてのみ、JSON オブジェクトを含めます。たとえば、Android プラットフォームのアプリ クライアントがない場合、ファイルの中に Android のエントリを含める必要はありません。
 
次の例には、現在受け入れられる有効なプラットフォーム ID のすべてが含まれています。 無効なプラットフォーム値が含まれる JSON オブジェクトは、除去されます。  

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

ID を検索するには:

* **windows_universal** - UWP アプリごとに 1 つの AUMID を提供します。 詳細については、「[インストール済みアプリのアプリケーション ユーザー モデル ID を検索する (Industry 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82))」および「[アプリケーション](https://docs.microsoft.com/ja-JP/uwp/schemas/appxpackage/appxmanifestschema/element-application)」を参照してください。
* **windows_win32** - アプリごとに 1 つの AUMID を提供します。 win32 アプリの場合、この情報を取得するにはスクリプトを使用する必要があります。 詳細については、「[インストール済みアプリのアプリケーション ユーザー モデル ID を検索する (Industry 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82))」を参照してください。
* **android** - 詳細については、「[パッケージ名の変更](https://developer.android.com/studio/build/application-id.html#change_the_package_name)」を参照してください。 
* **ios** - 詳細については、「[バンドル](https://developer.apple.com/documentation/foundation/bundle)」および「[必須プロパティ、ローカライズ可能なプロパティ、編集可能なプロパティ](https://help.apple.com/itunes-connect/developer/#/devfc3066644)」を参照してください。
* **msa** – [アプリケーション登録ポータル](https://apps.dev.microsoft.com)にサインインします。 自分の任意のアプリについて、アプリ ID/クライアント ID を確認できます。 Live SDK (16 進値) と統合アプリ ID (GUID) の両方がサポートされています。   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>手順 3: Microsoft アカウントまたは Azure AD のサポートを構成する
クロスデバイス エクスペリエンスを有効にするには、アプリ ユーザーが Microsoft アカウントまたは Azure AD アカウントのいずれかでサインインする必要があります。 クロスデバイス アプリ構成の一部として認証をサポートするためのアプリ ID/クライアント ID を提供することにより、クロスプラットフォーム サポートが有効になります。 最大 10 個のインスタンスを提供できます。

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

既存のアプリ ID/クライアント ID を検索するか、またはデベロッパー カウントで [アプリケーション登録ポータル](https://apps.dev.microsoft.com)にサインインすることにより新しい ID をプロビジョニングします。 サインインすると、自分の任意のアプリのアプリ ID/クライアント ID を確認できます。 Live SDK (16 進値) と統合アプリ ID (GUID) の両方がサポートされています。 前の例に示されているように、Microsoft アカウントまたは Azure AD のサポートを有効にするために使用される ID を追加する際には、プラットフォーム タイプとして "msa" を使用します。  

>**注:** Azure AD のユーザーをサポートするアプリケーションをビルドする場合、 [アプリケーション登録ポータル](https://apps.dev.microsoft.com)により発行される統合アプリケーション ID を使用していないなら、Azure アプリのアプリケーション ID のための GUID を提供することが必要になります。 このタイプの ID は、プラットフォーム タイプ "msa" としても構成されていなければなりません。 

テナントに対応する Azure Portal の GUID を検索するには: 

1. [Azure portal](https://portal.azure.com)にサインインします。
2. **Azure Active Directory** を選択します。 
3. **[管理]** の下で **[アプリの登録]** を選択します。
4. リストからアプリを選択します。 **[基本]** の下にアプリケーション ID (GUID) が表示されます。

#### <a name="encoding-the-cross-platform-app-identifiers-file"></a>cross-platform-app-identifiers ファイルのエンコード 
プラットフォームを移る際に、アクティビティが正しいネイティブ アプリケーションで再開しない場合、またはグループ内の全メンバーによって公開されているアクティビティを読み取ることができない場合、JSON ファイルが適切に解析されていないことが考えられます。 このファイルを出力する際には、cross-platform-app-identifiers ファイルを "Unicode (シグニチャなしの UTF-8) - コードページ 65001" エンコードで保存するようにしてください。

#### <a name="updating-the-cross-platform-app-identifiers-json-file"></a>cross-platform-app-identifiers JSON ファイルの更新 
ドメイン上で頻繁にリクエストが生成されるのを回避するため、JSON ファイルの内容はシステムによりキャッシュに入れられます。 構成されている場合、キャッシュ更新のタイミングを評価する際に、サービスにより HTTP キャッシュ ヘッダーが考慮されます。 構成されていない場合、サービスは 24 時間ごとに更新されます。 

## <a name="configure-your-app-client"></a>アプリ クライアントを構成する 
Windows、iOS、Android のクライアント サイド API を使用している場合、アプリ クライアントを確実に、クロスデバイス アプリ ID を表すホスト値 (contoso.com など) で構成する必要があります。

### <a name="microsoft-graph-apps"></a>Microsoft Graph のアプリ 
Microsoft Graph でアクティビティ フィード API を使用するアプリがある場合、ホスト値を **activitySourceHost** プロパティに指定する必要があります。 詳細については、「[アクティビティ リソース タイプ](/graph/api/resources/projectrome-activity?view=graph-rest-1.0)」を参照してください。

### <a name="universal-windows-apps"></a>ユニバーサル Windows アプリ
Windows アプリがある場合、データを公開する前に、アプリ マニフェストの中にホスト値を構成する必要があります。 詳細については、「[uap5:UserActivity](https://docs.microsoft.com/ja-JP/uwp/schemas/appxpackage/uapmanifestschema/element-uap5-useractivity)」を参照してください。 

<!-- Removing until we add the details.
### iOS & Android apps
*Details coming soon.*
-->

## <a name="maintaining-your-cross-device-app-configuration"></a>クロスデバイス アプリ構成のメンテナンス
ユーザー アクティビティを生成する新しいアプリケーションをリリースする際には、事前に新しい構成値を使用してクロスデバイス アプリを更新することが重要です。これにより、新たに公開されるアクティビティがある場合に、それらがクロスデバイス アプリに正しく関連付けられます。 構成に変更が加えられる前に公開されたユーザー アクティビティに関連付けられているクロスデバイス アプリ構成は、自動的には更新されません。 しかし、以前の構成のいずれかのアクティビティに対して更新操作が実行されると、ファイルの最新バージョンに更新されます。  

## <a name="troubleshooting"></a>トラブルシューティング

アクティビティ フィード API に関連してよく発生する問題として、次のものがあります。

### <a name="activities-are-not-available-to-read-and-write-for-all-apps-in-the-cross-device-app-configuration"></a>クロスデバイス アプリ構成のどのアプリについても、アクティビティを読み書き用に利用できない
アクティビティ フィード API はクロスデバイス アプリ構成を非同期に取り込むため、構成にエラーがあっても、ユーザー アクティビティの公開時に明らかにならないことがあります。 サービスで TLS や書式エラーのために JSON ファイルの取り込みに失敗した場合、公開されているアクティビティは、そのアクティビティを投稿したアプリ ID のみに帰属することになります。 アクティビティが Microsoft Graph によって公開されたものである場合、これは、Microsoft Graph へのリクエストを承認するために使用される Microsoft アカウント アプリ ID です。 アクティビティがクライアント サイド API によって公開されたものである場合、activity.applicationId は、アクティビティを投稿したプラットフォーム固有アプリの ID のみを記録します。 その場合、クロスデバイス アプリ構成の中で指定されている他のプラットフォーム固有アプリから、アクティビティに対して読み書きの操作を実行することはできません。 

### <a name="platform-will-not-initialize-on-android-or-ios"></a>Android または iOS でプラットフォームが初期化されない
Android または iOS のデバイス リレー API では、Android または iOS アプリへの接続のインスタンスを生成するために、クロスデバイス アプリ構成が必要です。 プラットフォームが正常に初期化できなかった場合は、Windows デベロッパー センターでクロスデバイス アプリを構成するために使用された Microsoft アカウント アプリ ID およびプッシュ通知認証情報が正しく指定されていることを確認した上で、クライアント アプリのホスト値を、クロスデバイス アプリを特定するドメインで構成してください。 
