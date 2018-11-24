# <a name="applisttype-enum-type"></a><span data-ttu-id="a8582-101">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a8582-101">appListType enum type</span></span>

> <span data-ttu-id="a8582-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a8582-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8582-103">準拠のアプリケーションのリストで使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="a8582-103">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="a8582-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8582-104">Members</span></span>
|<span data-ttu-id="a8582-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8582-105">Member</span></span>|<span data-ttu-id="a8582-106">値</span><span class="sxs-lookup"><span data-stu-id="a8582-106">Value</span></span>|<span data-ttu-id="a8582-107">説明</span><span class="sxs-lookup"><span data-stu-id="a8582-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8582-108">none</span><span class="sxs-lookup"><span data-stu-id="a8582-108">none</span></span>|<span data-ttu-id="a8582-109">0</span><span class="sxs-lookup"><span data-stu-id="a8582-109">0</span></span>|<span data-ttu-id="a8582-110">既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="a8582-110">Default value, no intent.</span></span>|
|<span data-ttu-id="a8582-111">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a8582-111">appsInListCompliant</span></span>|<span data-ttu-id="a8582-112">1</span><span class="sxs-lookup"><span data-stu-id="a8582-112">1</span></span>|<span data-ttu-id="a8582-113">一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="a8582-113">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="a8582-114">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a8582-114">appsNotInListCompliant</span></span>|<span data-ttu-id="a8582-115">2</span><span class="sxs-lookup"><span data-stu-id="a8582-115">2</span></span>|<span data-ttu-id="a8582-116">リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。</span><span class="sxs-lookup"><span data-stu-id="a8582-116">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



