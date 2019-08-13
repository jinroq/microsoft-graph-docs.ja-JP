---
title: win32LobAppFileSystemDetection リソースの種類
description: Win32 アプリを検出するためのファイルまたはフォルダーのパスが保存されています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd18cf615b33faa58e699bd53d93ed2110144c4a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335733"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="78af3-103">win32LobAppFileSystemDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78af3-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="78af3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78af3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78af3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78af3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78af3-106">Win32 アプリを検出するためのファイルまたはフォルダーのパスが保存されています。</span><span class="sxs-lookup"><span data-stu-id="78af3-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="78af3-107">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78af3-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78af3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78af3-108">Properties</span></span>
|<span data-ttu-id="78af3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78af3-109">Property</span></span>|<span data-ttu-id="78af3-110">型</span><span class="sxs-lookup"><span data-stu-id="78af3-110">Type</span></span>|<span data-ttu-id="78af3-111">説明</span><span class="sxs-lookup"><span data-stu-id="78af3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78af3-112">path</span><span class="sxs-lookup"><span data-stu-id="78af3-112">path</span></span>|<span data-ttu-id="78af3-113">String</span><span class="sxs-lookup"><span data-stu-id="78af3-113">String</span></span>|<span data-ttu-id="78af3-114">Win32 基幹業務 (LoB) アプリを検出するためのファイルまたはフォルダーのパス</span><span class="sxs-lookup"><span data-stu-id="78af3-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="78af3-115">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="78af3-115">fileOrFolderName</span></span>|<span data-ttu-id="78af3-116">String</span><span class="sxs-lookup"><span data-stu-id="78af3-116">String</span></span>|<span data-ttu-id="78af3-117">Win32 基幹業務 (LoB) アプリを検出するためのファイルまたはフォルダーの名前</span><span class="sxs-lookup"><span data-stu-id="78af3-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="78af3-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="78af3-118">check32BitOn64System</span></span>|<span data-ttu-id="78af3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="78af3-119">Boolean</span></span>|<span data-ttu-id="78af3-120">このファイルまたはフォルダーが、64ビットのシステム上の32ビット版アプリをチェックするためのものであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="78af3-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="78af3-121">detectionType</span><span class="sxs-lookup"><span data-stu-id="78af3-121">detectionType</span></span>|[<span data-ttu-id="78af3-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="78af3-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="78af3-123">ファイルシステムの検出の種類。</span><span class="sxs-lookup"><span data-stu-id="78af3-123">The file system detection type.</span></span> <span data-ttu-id="78af3-124">可能な値は、`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`、`doesNotExist` です。</span><span class="sxs-lookup"><span data-stu-id="78af3-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="78af3-125">operator</span><span class="sxs-lookup"><span data-stu-id="78af3-125">operator</span></span>|[<span data-ttu-id="78af3-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="78af3-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="78af3-127">ファイルまたはフォルダーの検出のための演算子。</span><span class="sxs-lookup"><span data-stu-id="78af3-127">The operator for file or folder detection.</span></span> <span data-ttu-id="78af3-128">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="78af3-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="78af3-129">detectionValue</span><span class="sxs-lookup"><span data-stu-id="78af3-129">detectionValue</span></span>|<span data-ttu-id="78af3-130">String</span><span class="sxs-lookup"><span data-stu-id="78af3-130">String</span></span>|<span data-ttu-id="78af3-131">ファイルまたはフォルダーの検出値</span><span class="sxs-lookup"><span data-stu-id="78af3-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="78af3-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78af3-132">Relationships</span></span>
<span data-ttu-id="78af3-133">なし</span><span class="sxs-lookup"><span data-stu-id="78af3-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78af3-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78af3-134">JSON Representation</span></span>
<span data-ttu-id="78af3-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78af3-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



