---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed27e057c6801bb1800f4ceb97bc74c779032dbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969682"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="db79b-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db79b-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="db79b-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="db79b-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db79b-106">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="db79b-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="db79b-107">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="db79b-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="db79b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db79b-108">Properties</span></span>
|<span data-ttu-id="db79b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db79b-109">Property</span></span>|<span data-ttu-id="db79b-110">種類</span><span class="sxs-lookup"><span data-stu-id="db79b-110">Type</span></span>|<span data-ttu-id="db79b-111">説明</span><span class="sxs-lookup"><span data-stu-id="db79b-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="db79b-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="db79b-112">Relationships</span></span>
<span data-ttu-id="db79b-113">なし</span><span class="sxs-lookup"><span data-stu-id="db79b-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="db79b-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db79b-114">JSON Representation</span></span>
<span data-ttu-id="db79b-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="db79b-115">Here is a JSON representation of the resource.</span></span>
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



