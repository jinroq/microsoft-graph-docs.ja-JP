# <a name="runstate-enum-type"></a><span data-ttu-id="cb810-101">runState 列挙型</span><span class="sxs-lookup"><span data-stu-id="cb810-101">runState enum type</span></span>

> <span data-ttu-id="cb810-102">**Important:** Microsoft Graph でのベータ (the / beta) バージョン の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cb810-102">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb810-103">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb810-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb810-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb810-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb810-105">デバイス管理スクリプトの実行ステータスの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="cb810-105">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="cb810-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="cb810-106">Members</span></span>
|<span data-ttu-id="cb810-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="cb810-107">Member</span></span>|<span data-ttu-id="cb810-108">値</span><span class="sxs-lookup"><span data-stu-id="cb810-108">Value</span></span>|<span data-ttu-id="cb810-109">説明</span><span class="sxs-lookup"><span data-stu-id="cb810-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb810-110">不明</span><span class="sxs-lookup"><span data-stu-id="cb810-110">unknown</span></span>|<span data-ttu-id="cb810-111">0</span><span class="sxs-lookup"><span data-stu-id="cb810-111">0%</span></span>|<span data-ttu-id="cb810-112">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="cb810-112">Unknown result.</span></span>|
|<span data-ttu-id="cb810-113">成功</span><span class="sxs-lookup"><span data-stu-id="cb810-113">success</span></span>|<span data-ttu-id="cb810-114">1</span><span class="sxs-lookup"><span data-stu-id="cb810-114">-1</span></span>|<span data-ttu-id="cb810-115">スクリプトが正常に実行します。</span><span class="sxs-lookup"><span data-stu-id="cb810-115">Script is run successfully.</span></span>|
|<span data-ttu-id="cb810-116">失敗</span><span class="sxs-lookup"><span data-stu-id="cb810-116">Fail</span></span>|<span data-ttu-id="cb810-117">2</span><span class="sxs-lookup"><span data-stu-id="cb810-117">-2</span></span>|<span data-ttu-id="cb810-118">スクリプトを実行できませんでした。</span><span class="sxs-lookup"><span data-stu-id="cb810-118">Script failed to run.</span></span>|



