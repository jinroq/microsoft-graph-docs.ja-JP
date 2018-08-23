# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="a1f54-101">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a1f54-101">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="a1f54-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1f54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1f54-103">要求されている Exchange Connector 同期の種類。</span><span class="sxs-lookup"><span data-stu-id="a1f54-103">The type of Exchange Connector Configured.</span></span>
## <a name="members"></a><span data-ttu-id="a1f54-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1f54-104">Members</span></span>
|<span data-ttu-id="a1f54-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1f54-105">Member</span></span>|<span data-ttu-id="a1f54-106">値</span><span class="sxs-lookup"><span data-stu-id="a1f54-106">Value</span></span>|<span data-ttu-id="a1f54-107">説明</span><span class="sxs-lookup"><span data-stu-id="a1f54-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1f54-108">fullSync</span><span class="sxs-lookup"><span data-stu-id="a1f54-108">fullSync</span></span>|<span data-ttu-id="a1f54-109">0</span><span class="sxs-lookup"><span data-stu-id="a1f54-109">0%</span></span>|<span data-ttu-id="a1f54-110">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="a1f54-110">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="a1f54-111">deltaSync</span><span class="sxs-lookup"><span data-stu-id="a1f54-111">deltaSync</span></span>|<span data-ttu-id="a1f54-112">1</span><span class="sxs-lookup"><span data-stu-id="a1f54-112">-1</span></span>|<span data-ttu-id="a1f54-113">差分同期ウィンドウ中に更新された Exchange 内のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="a1f54-113">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



