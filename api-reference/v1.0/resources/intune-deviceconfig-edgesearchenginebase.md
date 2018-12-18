---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
ms.openlocfilehash: ab7b02e9e158dd711347b27b916fc4bb97c1f2af
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301548"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="97d55-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97d55-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="97d55-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="97d55-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97d55-106">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="97d55-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="97d55-107">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="97d55-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="97d55-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97d55-108">Properties</span></span>
|<span data-ttu-id="97d55-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97d55-109">Property</span></span>|<span data-ttu-id="97d55-110">種類</span><span class="sxs-lookup"><span data-stu-id="97d55-110">Type</span></span>|<span data-ttu-id="97d55-111">説明</span><span class="sxs-lookup"><span data-stu-id="97d55-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="97d55-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97d55-112">Relationships</span></span>
<span data-ttu-id="97d55-113">なし</span><span class="sxs-lookup"><span data-stu-id="97d55-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97d55-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97d55-114">JSON Representation</span></span>
<span data-ttu-id="97d55-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97d55-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```



