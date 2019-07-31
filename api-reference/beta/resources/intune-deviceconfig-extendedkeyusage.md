---
title: extendedKeyUsage リソースの種類
description: カスタム拡張キー使用法の定義
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5fbcaaf764a0b079df77d81d07e53094a8035e07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001338"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="3a3c6-103">extendedKeyUsage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a3c6-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="3a3c6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a3c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a3c6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a3c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a3c6-106">カスタム拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="3a3c6-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="3a3c6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a3c6-107">Properties</span></span>
|<span data-ttu-id="3a3c6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a3c6-108">Property</span></span>|<span data-ttu-id="3a3c6-109">型</span><span class="sxs-lookup"><span data-stu-id="3a3c6-109">Type</span></span>|<span data-ttu-id="3a3c6-110">説明</span><span class="sxs-lookup"><span data-stu-id="3a3c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a3c6-111">name</span><span class="sxs-lookup"><span data-stu-id="3a3c6-111">name</span></span>|<span data-ttu-id="3a3c6-112">String</span><span class="sxs-lookup"><span data-stu-id="3a3c6-112">String</span></span>|<span data-ttu-id="3a3c6-113">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="3a3c6-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="3a3c6-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="3a3c6-114">objectIdentifier</span></span>|<span data-ttu-id="3a3c6-115">String</span><span class="sxs-lookup"><span data-stu-id="3a3c6-115">String</span></span>|<span data-ttu-id="3a3c6-116">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="3a3c6-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a3c6-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a3c6-117">Relationships</span></span>
<span data-ttu-id="3a3c6-118">なし</span><span class="sxs-lookup"><span data-stu-id="3a3c6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a3c6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a3c6-119">JSON Representation</span></span>
<span data-ttu-id="3a3c6-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a3c6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





