---
title: managementConditionExpression リソースの種類
description: 管理の条件式は、評価されるとき、つまり true または管理の条件付きステートメントがアクティブ/非アクティブであることを示す false のいずれかのブール値を生成する式です。 管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成されます。
ms.openlocfilehash: 68b0fdec3e1bf0db3d49040dbadfe9a7b1508cbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070516"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="0339a-104">managementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0339a-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="0339a-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0339a-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0339a-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0339a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0339a-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0339a-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0339a-108">管理の条件式は、評価されるとき、つまり true または管理の条件付きステートメントがアクティブ/非アクティブであることを示す false のいずれかのブール値を生成する式です。</span><span class="sxs-lookup"><span data-stu-id="0339a-108">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="0339a-109">管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成されます。</span><span class="sxs-lookup"><span data-stu-id="0339a-109">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>
## <a name="properties"></a><span data-ttu-id="0339a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0339a-110">Properties</span></span>
|<span data-ttu-id="0339a-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0339a-111">Property</span></span>|<span data-ttu-id="0339a-112">型</span><span class="sxs-lookup"><span data-stu-id="0339a-112">Type</span></span>|<span data-ttu-id="0339a-113">説明</span><span class="sxs-lookup"><span data-stu-id="0339a-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="0339a-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0339a-114">Relationships</span></span>
<span data-ttu-id="0339a-115">なし</span><span class="sxs-lookup"><span data-stu-id="0339a-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0339a-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0339a-116">JSON Representation</span></span>
<span data-ttu-id="0339a-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0339a-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpression"
}
```





