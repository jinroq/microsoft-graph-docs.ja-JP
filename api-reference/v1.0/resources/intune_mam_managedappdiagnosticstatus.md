# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="1f286-101">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f286-101">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="1f286-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f286-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f286-103">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="1f286-103">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="1f286-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f286-104">Properties</span></span>
|<span data-ttu-id="1f286-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f286-105">Property</span></span>|<span data-ttu-id="1f286-106">型</span><span class="sxs-lookup"><span data-stu-id="1f286-106">Type</span></span>|<span data-ttu-id="1f286-107">説明</span><span class="sxs-lookup"><span data-stu-id="1f286-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f286-108">validationName</span><span class="sxs-lookup"><span data-stu-id="1f286-108">validationName</span></span>|<span data-ttu-id="1f286-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1f286-109">String</span></span>|<span data-ttu-id="1f286-110">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="1f286-110">The validation friendly name</span></span>|
|<span data-ttu-id="1f286-111">state</span><span class="sxs-lookup"><span data-stu-id="1f286-111">state</span></span>|<span data-ttu-id="1f286-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1f286-112">String</span></span>|<span data-ttu-id="1f286-113">操作の状態</span><span class="sxs-lookup"><span data-stu-id="1f286-113">The state of the operation</span></span>|
|<span data-ttu-id="1f286-114">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="1f286-114">mitigationInstruction</span></span>|<span data-ttu-id="1f286-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1f286-115">String</span></span>|<span data-ttu-id="1f286-116">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="1f286-116">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f286-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f286-117">Relationships</span></span>
<span data-ttu-id="1f286-118">なし</span><span class="sxs-lookup"><span data-stu-id="1f286-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f286-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f286-119">JSON Representation</span></span>
<span data-ttu-id="1f286-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f286-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



