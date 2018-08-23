# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="992d8-101">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="992d8-101">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="992d8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="992d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="992d8-103">安全な検索（成人向けコンテンツのフィルタリング）が必要なレベルを指定します</span><span class="sxs-lookup"><span data-stu-id="992d8-103">Specifies what filter level of safe search is required.</span></span>
## <a name="members"></a><span data-ttu-id="992d8-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="992d8-104">Members</span></span>
|<span data-ttu-id="992d8-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="992d8-105">Member</span></span>|<span data-ttu-id="992d8-106">値</span><span class="sxs-lookup"><span data-stu-id="992d8-106">Value</span></span>|<span data-ttu-id="992d8-107">説明</span><span class="sxs-lookup"><span data-stu-id="992d8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="992d8-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="992d8-108">UserDefined</span></span>|<span data-ttu-id="992d8-109">0</span><span class="sxs-lookup"><span data-stu-id="992d8-109">0%</span></span>|<span data-ttu-id="992d8-110">ユーザー定義、デフォルト値、意図なし。</span><span class="sxs-lookup"><span data-stu-id="992d8-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="992d8-111">厳重</span><span class="sxs-lookup"><span data-stu-id="992d8-111">Strict</span></span>|<span data-ttu-id="992d8-112">1</span><span class="sxs-lookup"><span data-stu-id="992d8-112">-1</span></span>|<span data-ttu-id="992d8-113">大人のコンテンツに対する厳格かつ最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="992d8-113">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="992d8-114">中程度</span><span class="sxs-lookup"><span data-stu-id="992d8-114">Moderate</span></span>|<span data-ttu-id="992d8-115">2</span><span class="sxs-lookup"><span data-stu-id="992d8-115">-2</span></span>|<span data-ttu-id="992d8-116">アダルトコンテンツに対する適度なフィルタリング（有効な検索結果はフィルタリングされません）。</span><span class="sxs-lookup"><span data-stu-id="992d8-116">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



