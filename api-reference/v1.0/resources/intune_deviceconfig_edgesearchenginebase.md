# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="4099b-101">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4099b-101">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="4099b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4099b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4099b-103">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="4099b-103">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="4099b-104">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="4099b-104">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="4099b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4099b-105">Properties</span></span>
|<span data-ttu-id="4099b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4099b-106">Property</span></span>|<span data-ttu-id="4099b-107">型</span><span class="sxs-lookup"><span data-stu-id="4099b-107">Type</span></span>|<span data-ttu-id="4099b-108">説明</span><span class="sxs-lookup"><span data-stu-id="4099b-108">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="4099b-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4099b-109">Relationships</span></span>
<span data-ttu-id="4099b-110">なし</span><span class="sxs-lookup"><span data-stu-id="4099b-110">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4099b-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4099b-111">JSON Representation</span></span>
<span data-ttu-id="4099b-112">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4099b-112">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```








