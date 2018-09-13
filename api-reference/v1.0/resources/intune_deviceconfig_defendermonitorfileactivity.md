# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="59373-101">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="59373-101">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="59373-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59373-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59373-103">ファイル アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="59373-103">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="59373-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="59373-104">Members</span></span>
|<span data-ttu-id="59373-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="59373-105">Member</span></span>|<span data-ttu-id="59373-106">値</span><span class="sxs-lookup"><span data-stu-id="59373-106">Value</span></span>|<span data-ttu-id="59373-107">説明</span><span class="sxs-lookup"><span data-stu-id="59373-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59373-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="59373-108">UserDefined</span></span>|<span data-ttu-id="59373-109">0</span><span class="sxs-lookup"><span data-stu-id="59373-109">0%</span></span>|<span data-ttu-id="59373-110">ユーザー定義、デフォルト値、意図なし。</span><span class="sxs-lookup"><span data-stu-id="59373-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="59373-111">無効にする</span><span class="sxs-lookup"><span data-stu-id="59373-111">Disable</span></span>|<span data-ttu-id="59373-112">1</span><span class="sxs-lookup"><span data-stu-id="59373-112">-1</span></span>|<span data-ttu-id="59373-113">ファイル アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="59373-113">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="59373-114">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="59373-114">monitorAllFiles</span></span>|<span data-ttu-id="59373-115">2</span><span class="sxs-lookup"><span data-stu-id="59373-115">-2</span></span>|<span data-ttu-id="59373-116">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="59373-116">Monitor all files.</span></span>|
|<span data-ttu-id="59373-117">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="59373-117">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="59373-118">3</span><span class="sxs-lookup"><span data-stu-id="59373-118">"3"</span></span>| <span data-ttu-id="59373-119">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="59373-119">Monitor incoming files only.</span></span>|
|<span data-ttu-id="59373-120">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="59373-120">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="59373-121">4</span><span class="sxs-lookup"><span data-stu-id="59373-121">-4</span></span>|<span data-ttu-id="59373-122">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="59373-122">Monitor outgoing files only.</span></span>|








