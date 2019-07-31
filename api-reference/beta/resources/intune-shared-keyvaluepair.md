---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5d4a294be690e012d43893e44540658e919c123
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010428"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="123ac-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="123ac-103">keyValuePair resource type</span></span>

> <span data-ttu-id="123ac-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="123ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="123ac-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="123ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="123ac-106">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="123ac-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="123ac-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="123ac-107">Properties</span></span>
|<span data-ttu-id="123ac-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="123ac-108">Property</span></span>|<span data-ttu-id="123ac-109">型</span><span class="sxs-lookup"><span data-stu-id="123ac-109">Type</span></span>|<span data-ttu-id="123ac-110">説明</span><span class="sxs-lookup"><span data-stu-id="123ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="123ac-111">name</span><span class="sxs-lookup"><span data-stu-id="123ac-111">name</span></span>|<span data-ttu-id="123ac-112">String</span><span class="sxs-lookup"><span data-stu-id="123ac-112">String</span></span>|<span data-ttu-id="123ac-113">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="123ac-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="123ac-114">value</span><span class="sxs-lookup"><span data-stu-id="123ac-114">value</span></span>|<span data-ttu-id="123ac-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="123ac-115">String</span></span>|<span data-ttu-id="123ac-116">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="123ac-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="123ac-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="123ac-117">Relationships</span></span>
<span data-ttu-id="123ac-118">なし</span><span class="sxs-lookup"><span data-stu-id="123ac-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="123ac-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="123ac-119">JSON Representation</span></span>
<span data-ttu-id="123ac-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="123ac-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```





