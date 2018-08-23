# <a name="applisttype-enum-type"></a><span data-ttu-id="ab4e5-101">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ab4e5-101">appListType enum type</span></span>

> <span data-ttu-id="ab4e5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab4e5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab4e5-103">コンプライアンス アプリ リストの使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="ab4e5-103">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="ab4e5-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab4e5-104">Members</span></span>
|<span data-ttu-id="ab4e5-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab4e5-105">Member</span></span>|<span data-ttu-id="ab4e5-106">値</span><span class="sxs-lookup"><span data-stu-id="ab4e5-106">Value</span></span>|<span data-ttu-id="ab4e5-107">説明</span><span class="sxs-lookup"><span data-stu-id="ab4e5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab4e5-108">none</span><span class="sxs-lookup"><span data-stu-id="ab4e5-108">none</span></span>|<span data-ttu-id="ab4e5-109">0</span><span class="sxs-lookup"><span data-stu-id="ab4e5-109">0%</span></span>|<span data-ttu-id="ab4e5-110">規定値、目的なし。</span><span class="sxs-lookup"><span data-stu-id="ab4e5-110">Default value, no intent.</span></span>|
|<span data-ttu-id="ab4e5-111">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="ab4e5-111">appsInListCompliant</span></span>|<span data-ttu-id="ab4e5-112">1</span><span class="sxs-lookup"><span data-stu-id="ab4e5-112">-1</span></span>|<span data-ttu-id="ab4e5-113">リストはコンプライアンスに準拠すると見なされるアプリを表示（リスト上のアプリのみがコンプライアンスに準拠）。</span><span class="sxs-lookup"><span data-stu-id="ab4e5-113">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="ab4e5-114">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="ab4e5-114">appsNotInListCompliant</span></span>|<span data-ttu-id="ab4e5-115">2</span><span class="sxs-lookup"><span data-stu-id="ab4e5-115">-2</span></span>|<span data-ttu-id="ab4e5-116">リストはコンプライアンスに準拠しないと見なされるアプリを表示（リストに表示されているアプリ以外はコンプライアンスに準拠）。</span><span class="sxs-lookup"><span data-stu-id="ab4e5-116">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



