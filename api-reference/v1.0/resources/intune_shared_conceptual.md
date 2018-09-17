# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="b16bd-101">Microsoft Intune 内の共有リソース</span><span class="sxs-lookup"><span data-stu-id="b16bd-101">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="b16bd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b16bd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b16bd-103">これらのエンドポイントは、Intune ワークフローの複数の Microsoft Graph API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b16bd-103">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="b16bd-104">所与のリソースを使用する意図、目的、必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="b16bd-104">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="b16bd-105">さらに、特定のワークフローに対してのみサポートされているメソッド、プロパティ、アクションもあります。</span><span class="sxs-lookup"><span data-stu-id="b16bd-105">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="b16bd-106">次の Graph リソースは、Intune ワークフロー間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="b16bd-106">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="b16bd-107">すべてのデバイスの割り当て先</span><span class="sxs-lookup"><span data-stu-id="b16bd-107">All devices assignment target</span></span>](intune_shared_alldevicesassignmenttarget.md)
- [<span data-ttu-id="b16bd-108">すべてのライセンス ユーザーの割り当て先</span><span class="sxs-lookup"><span data-stu-id="b16bd-108">All licensed users assignment target</span></span>](intune_shared_alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="b16bd-109">コンプライアンスの状況</span><span class="sxs-lookup"><span data-stu-id="b16bd-109">Compliance status</span></span>](intune_shared_compliancestatus.md)
- [<span data-ttu-id="b16bd-110">デバイスおよびアプリ管理の割り当て先</span><span class="sxs-lookup"><span data-stu-id="b16bd-110">Device and app management assignment target</span></span>](intune_shared_deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="b16bd-111">デバイス アプリの管理</span><span class="sxs-lookup"><span data-stu-id="b16bd-111">Device app management</span></span>](intune_shared_deviceappmanagement.md)
- [<span data-ttu-id="b16bd-112">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="b16bd-112">Device category</span></span>](intune_shared_devicecategory.md)
- <span data-ttu-id="b16bd-113">[デバイス登録の種類](intune_shared_deviceenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="b16bd-113">For [Device enrollment](intune_shared_deviceenrollmenttype.md) type, choose Managed apps.</span></span>
- [<span data-ttu-id="b16bd-114">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="b16bd-114">Device management</span></span>](intune_shared_devicemanagement.md)
- [<span data-ttu-id="b16bd-115">除外グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="b16bd-115">Exclusion group assignment target</span></span>](intune_shared_exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="b16bd-116">グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="b16bd-116">Group assignment target</span></span>](intune_shared_groupassignmenttarget.md)
- [<span data-ttu-id="b16bd-117">目的をインストールします</span><span class="sxs-lookup"><span data-stu-id="b16bd-117">Install intent</span></span>](intune_shared_installintent.md)
- [<span data-ttu-id="b16bd-118">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="b16bd-118">MIME content</span></span>](intune_shared_mimecontent.md)
- [<span data-ttu-id="b16bd-119">レポート</span><span class="sxs-lookup"><span data-stu-id="b16bd-119">Report</span></span>](intune_shared_report.md)
- [<span data-ttu-id="b16bd-120">レポートのルート</span><span class="sxs-lookup"><span data-stu-id="b16bd-120">Report root</span></span>](intune_shared_reportroot.md)
- [<span data-ttu-id="b16bd-121">UI 状態の生成オプションを保存しました</span><span class="sxs-lookup"><span data-stu-id="b16bd-121">Saved UI state generation options</span></span>](intune_shared_saveduistategenerationoptions.md)
- [<span data-ttu-id="b16bd-122">URI</span><span class="sxs-lookup"><span data-stu-id="b16bd-122">URI</span></span>](intune_shared_uri.md)
- [<span data-ttu-id="b16bd-123">ユーザー</span><span class="sxs-lookup"><span data-stu-id="b16bd-123">User</span></span>](intune_shared_user.md)
- [<span data-ttu-id="b16bd-124">VPP トークン アカウントの種類</span><span class="sxs-lookup"><span data-stu-id="b16bd-124">VPP token account type</span></span>](intune_shared_vpptokenaccounttype.md)
