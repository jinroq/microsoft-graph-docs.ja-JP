# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="7f13b-101">applicationGuardBlockClipboardSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7f13b-101">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="7f13b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f13b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f13b-103">ApplicationGuardBlockClipboardSharingType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="7f13b-103">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="7f13b-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="7f13b-104">Members</span></span>
|<span data-ttu-id="7f13b-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="7f13b-105">Member</span></span>|<span data-ttu-id="7f13b-106">値</span><span class="sxs-lookup"><span data-stu-id="7f13b-106">Value</span></span>|<span data-ttu-id="7f13b-107">説明</span><span class="sxs-lookup"><span data-stu-id="7f13b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f13b-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7f13b-108">notConfigured</span></span>|<span data-ttu-id="7f13b-109">0</span><span class="sxs-lookup"><span data-stu-id="7f13b-109">0%</span></span>|<span data-ttu-id="7f13b-110">未構成</span><span class="sxs-lookup"><span data-stu-id="7f13b-110">Not configured</span></span>|
|<span data-ttu-id="7f13b-111">blockBoth</span><span class="sxs-lookup"><span data-stu-id="7f13b-111">blockBoth</span></span>|<span data-ttu-id="7f13b-112">1</span><span class="sxs-lookup"><span data-stu-id="7f13b-112">-1</span></span>|<span data-ttu-id="7f13b-113">ホストからコンテナー、コンテナーからホストへの両方のデータを共有するためにクリップボード をブロックする</span><span class="sxs-lookup"><span data-stu-id="7f13b-113">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|
|<span data-ttu-id="7f13b-114">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="7f13b-114">blockHostToContainer</span></span>|<span data-ttu-id="7f13b-115">2</span><span class="sxs-lookup"><span data-stu-id="7f13b-115">-2</span></span>|<span data-ttu-id="7f13b-116">ホストからコンテナーへのデータを共有するためにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="7f13b-116">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|
|<span data-ttu-id="7f13b-117">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="7f13b-117">blockContainerToHost</span></span>|<span data-ttu-id="7f13b-118">3</span><span class="sxs-lookup"><span data-stu-id="7f13b-118">"3"</span></span>|<span data-ttu-id="7f13b-119">コンテナーからホストへのデータを共有するためにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="7f13b-119">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|
|<span data-ttu-id="7f13b-120">blockNone</span><span class="sxs-lookup"><span data-stu-id="7f13b-120">blockNone</span></span>|<span data-ttu-id="7f13b-121">4</span><span class="sxs-lookup"><span data-stu-id="7f13b-121">-4</span></span>|<span data-ttu-id="7f13b-122">ホストからコンテナー、コンテナーからホストへのデータを共有するクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="7f13b-122">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|








