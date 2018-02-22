# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="675a3-101">Microsoft Graph での Intune の操作</span><span class="sxs-lookup"><span data-stu-id="675a3-101">Working with files in Microsoft Graph</span></span>  

> <span data-ttu-id="675a3-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/ja-JP/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="675a3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/ja-JP/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="675a3-103">Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="675a3-103">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="675a3-104">モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/ja-JP/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="675a3-104">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/ja-JP/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="675a3-105">Intune Graph API の使用</span><span class="sxs-lookup"><span data-stu-id="675a3-105">Using the Intune Graph API</span></span>

<span data-ttu-id="675a3-106">Intune は、豊富なエンティティ情報とリレーションシップのナビゲーションを使用して、他のクラウド サービスと同じ方法で Microsoft Graph API にデータを提供します。</span><span class="sxs-lookup"><span data-stu-id="675a3-106">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span>  <span data-ttu-id="675a3-107">Microsoft Graph API を使用して、他のサービスからの情報と Intune を結合し、IT プロフェッショナルやエンド ユーザー向けの豊富なサービス間アプリケーションをビルドします。</span><span class="sxs-lookup"><span data-stu-id="675a3-107">Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="675a3-108">以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="675a3-108">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="675a3-109">Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="675a3-109">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    <span data-ttu-id="675a3-110">https://graph.microsoft.com/users/{user}/ownedDevices</span><span class="sxs-lookup"><span data-stu-id="675a3-110">https://graph.microsoft.com/beta/administrativeUnits</span></span> 

2. <span data-ttu-id="675a3-111">次に、テナントのアプリケーションのリストを表示します。</span><span class="sxs-lookup"><span data-stu-id="675a3-111">Then view the list of applications for your tenant:</span></span> 

    <span data-ttu-id="675a3-112">https://graph.microsoft.com/deviceAppManagement/mobileApps</span><span class="sxs-lookup"><span data-stu-id="675a3-112">https://graph.microsoft.com/beta/administrativeUnits</span></span>  

3. <span data-ttu-id="675a3-113">アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="675a3-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    <span data-ttu-id="675a3-114">https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/</span><span class="sxs-lookup"><span data-stu-id="675a3-114">https://graph.microsoft.com/beta/administrativeUnits</span></span>


## <a name="using-permission-scopes"></a><span data-ttu-id="675a3-115">アクセス許可のスコープの使用</span><span class="sxs-lookup"><span data-stu-id="675a3-115">Using permission scopes</span></span>

<span data-ttu-id="675a3-116">Microsoft Graph API では、アクセス許可のスコープによってリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="675a3-116">Microsoft Graph API controls access to resources using permission scopes.</span></span> <span data-ttu-id="675a3-117">開発者は、Intune リソースにアクセスするために必要となる、アクセス許可のスコープを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="675a3-117">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="675a3-118">通常は Azure Active Directory ポータルで必要なアクセス許可のスコープを指定します。</span><span class="sxs-lookup"><span data-stu-id="675a3-118">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="675a3-119">詳細については、「[Microsoft Graph のアクセス許可スコープ](https://developer.microsoft.com/ja-JP/graph/docs/authorization/permission_scopes)」および「[Intune のアクセス許可のスコープ](https://developer.microsoft.com/ja-JP/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="675a3-119">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/ja-JP/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/ja-JP/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

