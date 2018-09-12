# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="a1952-101">managedAppClipboardSharingLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="a1952-101">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="a1952-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1952-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1952-103">アプリケーションとの間でデバイスのクリップボードを共有する可能性があるレベルを表します</span><span class="sxs-lookup"><span data-stu-id="a1952-103">The level to which the clipboard may be shared between apps on the managed device.</span></span>
## <a name="members"></a><span data-ttu-id="a1952-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1952-104">Members</span></span>
|<span data-ttu-id="a1952-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1952-105">Member</span></span>|<span data-ttu-id="a1952-106">値</span><span class="sxs-lookup"><span data-stu-id="a1952-106">Value</span></span>|<span data-ttu-id="a1952-107">説明</span><span class="sxs-lookup"><span data-stu-id="a1952-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1952-108">allApps</span><span class="sxs-lookup"><span data-stu-id="a1952-108">allApps</span></span>|<span data-ttu-id="a1952-109">0</span><span class="sxs-lookup"><span data-stu-id="a1952-109">0%</span></span>|<span data-ttu-id="a1952-110">共有はすべてのアプリケーション間で管理するしないかを許可されます</span><span class="sxs-lookup"><span data-stu-id="a1952-110">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="a1952-111">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="a1952-111">managedAppsWithPasteIn</span></span>|<span data-ttu-id="a1952-112">1</span><span class="sxs-lookup"><span data-stu-id="a1952-112">-1</span></span>|<span data-ttu-id="a1952-113">共有は、貼り付けが有効になっている管理されるすべてのアプリケーションの間で許可されます。</span><span class="sxs-lookup"><span data-stu-id="a1952-113">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="a1952-114">managedApps</span><span class="sxs-lookup"><span data-stu-id="a1952-114">managedApps</span></span>|<span data-ttu-id="a1952-115">2</span><span class="sxs-lookup"><span data-stu-id="a1952-115">-2</span></span>|<span data-ttu-id="a1952-116">共有はすべての管理されるアプリケーションの間で許可されます</span><span class="sxs-lookup"><span data-stu-id="a1952-116">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="a1952-117">ブロックされています</span><span class="sxs-lookup"><span data-stu-id="a1952-117">blocked</span></span>|<span data-ttu-id="a1952-118">3</span><span class="sxs-lookup"><span data-stu-id="a1952-118">"3"</span></span>|<span data-ttu-id="a1952-119">アプリケーション間の共有が無効になっています</span><span class="sxs-lookup"><span data-stu-id="a1952-119">Sharing between apps is disabled</span></span>|








