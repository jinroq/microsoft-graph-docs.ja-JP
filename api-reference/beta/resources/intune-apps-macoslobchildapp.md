---
title: macOSLobChildApp リソースの種類
description: バンドルパッケージ内の MacOS LOB アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ca4d371966781378c9097769d9178de69d8f7d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012591"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="6d911-103">macOSLobChildApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d911-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="6d911-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d911-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d911-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d911-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d911-106">バンドルパッケージ内の MacOS LOB アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d911-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="6d911-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d911-107">Properties</span></span>
|<span data-ttu-id="6d911-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d911-108">Property</span></span>|<span data-ttu-id="6d911-109">型</span><span class="sxs-lookup"><span data-stu-id="6d911-109">Type</span></span>|<span data-ttu-id="6d911-110">説明</span><span class="sxs-lookup"><span data-stu-id="6d911-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d911-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="6d911-111">bundleId</span></span>|<span data-ttu-id="6d911-112">String</span><span class="sxs-lookup"><span data-stu-id="6d911-112">String</span></span>|<span data-ttu-id="6d911-113">ID 名。</span><span class="sxs-lookup"><span data-stu-id="6d911-113">The Identity Name.</span></span>|
|<span data-ttu-id="6d911-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="6d911-114">buildNumber</span></span>|<span data-ttu-id="6d911-115">String</span><span class="sxs-lookup"><span data-stu-id="6d911-115">String</span></span>|<span data-ttu-id="6d911-116">MacOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="6d911-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6d911-117">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="6d911-117">versionNumber</span></span>|<span data-ttu-id="6d911-118">String</span><span class="sxs-lookup"><span data-stu-id="6d911-118">String</span></span>|<span data-ttu-id="6d911-119">MacOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="6d911-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d911-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d911-120">Relationships</span></span>
<span data-ttu-id="6d911-121">なし</span><span class="sxs-lookup"><span data-stu-id="6d911-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d911-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d911-122">JSON Representation</span></span>
<span data-ttu-id="6d911-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6d911-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





