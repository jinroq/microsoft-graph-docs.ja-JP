---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: c58865e746afcde8167c8d905c3b4064d8690a95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309186"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="9c629-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c629-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="9c629-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c629-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c629-105">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9c629-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="9c629-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c629-106">Properties</span></span>
|<span data-ttu-id="9c629-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c629-107">Property</span></span>|<span data-ttu-id="9c629-108">種類</span><span class="sxs-lookup"><span data-stu-id="9c629-108">Type</span></span>|<span data-ttu-id="9c629-109">説明</span><span class="sxs-lookup"><span data-stu-id="9c629-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c629-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="9c629-110">encryptionKey</span></span>|<span data-ttu-id="9c629-111">Binary</span><span class="sxs-lookup"><span data-stu-id="9c629-111">Binary</span></span>|<span data-ttu-id="9c629-112">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="9c629-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="9c629-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="9c629-113">initializationVector</span></span>|<span data-ttu-id="9c629-114">Binary</span><span class="sxs-lookup"><span data-stu-id="9c629-114">Binary</span></span>|<span data-ttu-id="9c629-115">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="9c629-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="9c629-116">Mac</span><span class="sxs-lookup"><span data-stu-id="9c629-116">mac</span></span>|<span data-ttu-id="9c629-117">Binary</span><span class="sxs-lookup"><span data-stu-id="9c629-117">Binary</span></span>|<span data-ttu-id="9c629-118">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="9c629-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="9c629-119">macKey</span><span class="sxs-lookup"><span data-stu-id="9c629-119">macKey</span></span>|<span data-ttu-id="9c629-120">Binary</span><span class="sxs-lookup"><span data-stu-id="9c629-120">Binary</span></span>|<span data-ttu-id="9c629-121">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="9c629-121">The key used to get mac.</span></span>|
|<span data-ttu-id="9c629-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="9c629-122">profileIdentifier</span></span>|<span data-ttu-id="9c629-123">String</span><span class="sxs-lookup"><span data-stu-id="9c629-123">String</span></span>|<span data-ttu-id="9c629-124">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="9c629-124">The the profile identifier.</span></span>|
|<span data-ttu-id="9c629-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="9c629-125">fileDigest</span></span>|<span data-ttu-id="9c629-126">Binary</span><span class="sxs-lookup"><span data-stu-id="9c629-126">Binary</span></span>|<span data-ttu-id="9c629-127">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="9c629-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="9c629-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="9c629-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="9c629-129">String</span><span class="sxs-lookup"><span data-stu-id="9c629-129">String</span></span>|<span data-ttu-id="9c629-130">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="9c629-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c629-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c629-131">Relationships</span></span>
<span data-ttu-id="9c629-132">なし</span><span class="sxs-lookup"><span data-stu-id="9c629-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c629-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c629-133">JSON Representation</span></span>
<span data-ttu-id="9c629-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c629-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



