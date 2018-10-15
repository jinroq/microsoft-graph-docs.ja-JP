# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="ca9a2-101">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="ca9a2-101">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="ca9a2-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca9a2-103">診断データと利用統計情報データ (Watson など) の送信をデバイスに許可します。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-103">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="ca9a2-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="ca9a2-104">Members</span></span>
|<span data-ttu-id="ca9a2-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="ca9a2-105">Member</span></span>|<span data-ttu-id="ca9a2-106">値</span><span class="sxs-lookup"><span data-stu-id="ca9a2-106">Value</span></span>|<span data-ttu-id="ca9a2-107">説明</span><span class="sxs-lookup"><span data-stu-id="ca9a2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca9a2-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="ca9a2-108">UserDefined</span></span>|<span data-ttu-id="ca9a2-109">0</span><span class="sxs-lookup"><span data-stu-id="ca9a2-109">0%</span></span>|<span data-ttu-id="ca9a2-110">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-110">Allow the user to set.</span></span>|
|<span data-ttu-id="ca9a2-111">なし</span><span class="sxs-lookup"><span data-stu-id="ca9a2-111">none</span></span>|<span data-ttu-id="ca9a2-112">1</span><span class="sxs-lookup"><span data-stu-id="ca9a2-112">-1</span></span>|<span data-ttu-id="ca9a2-113">OS コンポーネントからは、利用統計情報は送信されません。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-113">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="ca9a2-114">注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-114">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="ca9a2-115">その他のデバイスでこの設定を使用することは、1 の値を設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-115">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="ca9a2-116">基本</span><span class="sxs-lookup"><span data-stu-id="ca9a2-116">Basic</span></span>|<span data-ttu-id="ca9a2-117">2</span><span class="sxs-lookup"><span data-stu-id="ca9a2-117">-2</span></span>|<span data-ttu-id="ca9a2-118">基本的な利用統計情報を送信します。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-118">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="ca9a2-119">強化</span><span class="sxs-lookup"><span data-stu-id="ca9a2-119">Enhanced</span></span>|<span data-ttu-id="ca9a2-120">3</span><span class="sxs-lookup"><span data-stu-id="ca9a2-120">"3"</span></span>|<span data-ttu-id="ca9a2-121">使用状況とインサイトデータを含む強化された利用統計情報を送信します。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-121">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="ca9a2-122">フル</span><span class="sxs-lookup"><span data-stu-id="ca9a2-122">Full</span></span>|<span data-ttu-id="ca9a2-123">4</span><span class="sxs-lookup"><span data-stu-id="ca9a2-123">-4</span></span>|<span data-ttu-id="ca9a2-124">システム状態などの診断データを含む完全な利用統計情報を送信します。</span><span class="sxs-lookup"><span data-stu-id="ca9a2-124">Sends full telemetry data including diagnostic data, such as system state.</span></span>|








