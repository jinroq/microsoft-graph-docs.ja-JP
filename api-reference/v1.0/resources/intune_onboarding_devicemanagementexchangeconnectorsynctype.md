# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="6dc61-101">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6dc61-101">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="6dc61-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6dc61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dc61-103">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="6dc61-103">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="6dc61-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="6dc61-104">Members</span></span>
|<span data-ttu-id="6dc61-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="6dc61-105">Member</span></span>|<span data-ttu-id="6dc61-106">値</span><span class="sxs-lookup"><span data-stu-id="6dc61-106">Value</span></span>|<span data-ttu-id="6dc61-107">説明</span><span class="sxs-lookup"><span data-stu-id="6dc61-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc61-108">fullSync</span><span class="sxs-lookup"><span data-stu-id="6dc61-108">fullSync</span></span>|<span data-ttu-id="6dc61-109">0</span><span class="sxs-lookup"><span data-stu-id="6dc61-109">0</span></span>|<span data-ttu-id="6dc61-110">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="6dc61-110">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="6dc61-111">deltaSync</span><span class="sxs-lookup"><span data-stu-id="6dc61-111">deltaSync</span></span>|<span data-ttu-id="6dc61-112">1</span><span class="sxs-lookup"><span data-stu-id="6dc61-112">1</span></span>|<span data-ttu-id="6dc61-113">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="6dc61-113">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



