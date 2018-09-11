# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="f8f82-101">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="f8f82-101">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="f8f82-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8f82-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8f82-103">Windows ユーザー アカウントに使用できる値は、設定を制御します。</span><span class="sxs-lookup"><span data-stu-id="f8f82-103">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="f8f82-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8f82-104">Members</span></span>
|<span data-ttu-id="f8f82-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8f82-105">Member</span></span>|<span data-ttu-id="f8f82-106">値</span><span class="sxs-lookup"><span data-stu-id="f8f82-106">Value</span></span>|<span data-ttu-id="f8f82-107">説明</span><span class="sxs-lookup"><span data-stu-id="f8f82-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8f82-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="f8f82-108">UserDefined</span></span>|<span data-ttu-id="f8f82-109">0</span><span class="sxs-lookup"><span data-stu-id="f8f82-109">0%</span></span>|<span data-ttu-id="f8f82-110">ユーザー定義、デフォルト値、意図なし。</span><span class="sxs-lookup"><span data-stu-id="f8f82-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f8f82-111">AlwaysNotify</span><span class="sxs-lookup"><span data-stu-id="f8f82-111">AlwaysNotify</span></span>|<span data-ttu-id="f8f82-112">1</span><span class="sxs-lookup"><span data-stu-id="f8f82-112">-1</span></span>|<span data-ttu-id="f8f82-113">常に次のように通知します。</span><span class="sxs-lookup"><span data-stu-id="f8f82-113">Always notify.</span></span>|
|<span data-ttu-id="f8f82-114">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="f8f82-114">notifyOnAppChanges</span></span>|<span data-ttu-id="f8f82-115">2</span><span class="sxs-lookup"><span data-stu-id="f8f82-115">-2</span></span>|<span data-ttu-id="f8f82-116">アプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="f8f82-116">Notify on app changes.</span></span>|
|<span data-ttu-id="f8f82-117">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="f8f82-117">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="f8f82-118">3</span><span class="sxs-lookup"><span data-stu-id="f8f82-118">"3"</span></span>|<span data-ttu-id="f8f82-119">デスクトップを暗転しないアプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="f8f82-119">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="f8f82-120">neverNotify</span><span class="sxs-lookup"><span data-stu-id="f8f82-120">neverNotify</span></span>|<span data-ttu-id="f8f82-121">4</span><span class="sxs-lookup"><span data-stu-id="f8f82-121">-4</span></span>|<span data-ttu-id="f8f82-122">通知しません。</span><span class="sxs-lookup"><span data-stu-id="f8f82-122">Never notify.</span></span>|








