---
title: win32LobAppFileSystemRequirement リソースの種類
description: Win32 アプリを検出するためのファイルまたはフォルダーのパスが保存されています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f57206e7fda4eedb55be1e4ceba89323084289dc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335698"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="7afb7-103">win32LobAppFileSystemRequirement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7afb7-103">win32LobAppFileSystemRequirement resource type</span></span>

> <span data-ttu-id="7afb7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7afb7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7afb7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7afb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7afb7-106">Win32 アプリを検出するためのファイルまたはフォルダーのパスが保存されています。</span><span class="sxs-lookup"><span data-stu-id="7afb7-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="7afb7-107">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7afb7-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7afb7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7afb7-108">Properties</span></span>
|<span data-ttu-id="7afb7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7afb7-109">Property</span></span>|<span data-ttu-id="7afb7-110">型</span><span class="sxs-lookup"><span data-stu-id="7afb7-110">Type</span></span>|<span data-ttu-id="7afb7-111">説明</span><span class="sxs-lookup"><span data-stu-id="7afb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7afb7-112">operator</span><span class="sxs-lookup"><span data-stu-id="7afb7-112">operator</span></span>|[<span data-ttu-id="7afb7-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="7afb7-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="7afb7-114">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出の演算子。</span><span class="sxs-lookup"><span data-stu-id="7afb7-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="7afb7-115">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="7afb7-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="7afb7-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="7afb7-116">detectionValue</span></span>|<span data-ttu-id="7afb7-117">String</span><span class="sxs-lookup"><span data-stu-id="7afb7-117">String</span></span>|<span data-ttu-id="7afb7-118">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出値</span><span class="sxs-lookup"><span data-stu-id="7afb7-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="7afb7-119">path</span><span class="sxs-lookup"><span data-stu-id="7afb7-119">path</span></span>|<span data-ttu-id="7afb7-120">String</span><span class="sxs-lookup"><span data-stu-id="7afb7-120">String</span></span>|<span data-ttu-id="7afb7-121">Win32 基幹業務 (LoB) アプリを検出するためのファイルまたはフォルダーのパス</span><span class="sxs-lookup"><span data-stu-id="7afb7-121">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="7afb7-122">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="7afb7-122">fileOrFolderName</span></span>|<span data-ttu-id="7afb7-123">String</span><span class="sxs-lookup"><span data-stu-id="7afb7-123">String</span></span>|<span data-ttu-id="7afb7-124">Win32 基幹業務 (LoB) アプリを検出するためのファイルまたはフォルダーの名前</span><span class="sxs-lookup"><span data-stu-id="7afb7-124">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="7afb7-125">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="7afb7-125">check32BitOn64System</span></span>|<span data-ttu-id="7afb7-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="7afb7-126">Boolean</span></span>|<span data-ttu-id="7afb7-127">このファイルまたはフォルダーが、64ビットのシステム上の32ビット版アプリをチェックするためのものであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7afb7-127">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="7afb7-128">detectionType</span><span class="sxs-lookup"><span data-stu-id="7afb7-128">detectionType</span></span>|[<span data-ttu-id="7afb7-129">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="7afb7-129">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="7afb7-130">ファイルシステムの検出の種類。</span><span class="sxs-lookup"><span data-stu-id="7afb7-130">The file system detection type.</span></span> <span data-ttu-id="7afb7-131">可能な値は、`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`、`doesNotExist` です。</span><span class="sxs-lookup"><span data-stu-id="7afb7-131">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7afb7-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7afb7-132">Relationships</span></span>
<span data-ttu-id="7afb7-133">なし</span><span class="sxs-lookup"><span data-stu-id="7afb7-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7afb7-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7afb7-134">JSON Representation</span></span>
<span data-ttu-id="7afb7-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7afb7-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRequirement",
  "operator": "String",
  "detectionValue": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String"
}
```



