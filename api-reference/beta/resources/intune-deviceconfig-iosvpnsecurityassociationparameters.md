---
title: iosVpnSecurityAssociationParameters リソースの種類
description: VPN セキュリティアソシエーションのパラメーター
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ecf2597222a578d342f69c16c665c493b8c3329
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002729"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="3d7a3-103">iosVpnSecurityAssociationParameters リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d7a3-103">iosVpnSecurityAssociationParameters resource type</span></span>

> <span data-ttu-id="3d7a3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d7a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d7a3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3d7a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d7a3-106">VPN セキュリティアソシエーションのパラメーター</span><span class="sxs-lookup"><span data-stu-id="3d7a3-106">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="3d7a3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d7a3-107">Properties</span></span>
|<span data-ttu-id="3d7a3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d7a3-108">Property</span></span>|<span data-ttu-id="3d7a3-109">型</span><span class="sxs-lookup"><span data-stu-id="3d7a3-109">Type</span></span>|<span data-ttu-id="3d7a3-110">説明</span><span class="sxs-lookup"><span data-stu-id="3d7a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d7a3-111">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3d7a3-111">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="3d7a3-112">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="3d7a3-112">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="3d7a3-113">暗号化アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="3d7a3-113">Encryption algorithm.</span></span> <span data-ttu-id="3d7a3-114">使用可能な値: `aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`。</span><span class="sxs-lookup"><span data-stu-id="3d7a3-114">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="3d7a3-115">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3d7a3-115">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="3d7a3-116">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="3d7a3-116">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="3d7a3-117">整合性アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="3d7a3-117">Integrity algorithm.</span></span> <span data-ttu-id="3d7a3-118">可能な値は、`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512` です。</span><span class="sxs-lookup"><span data-stu-id="3d7a3-118">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="3d7a3-119">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="3d7a3-119">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="3d7a3-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3d7a3-120">Int32</span></span>|<span data-ttu-id="3d7a3-121">Diffie-hellman グループ</span><span class="sxs-lookup"><span data-stu-id="3d7a3-121">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="3d7a3-122">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="3d7a3-122">lifetimeInMinutes</span></span>|<span data-ttu-id="3d7a3-123">Int32</span><span class="sxs-lookup"><span data-stu-id="3d7a3-123">Int32</span></span>|<span data-ttu-id="3d7a3-124">有効期間 (分)</span><span class="sxs-lookup"><span data-stu-id="3d7a3-124">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d7a3-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3d7a3-125">Relationships</span></span>
<span data-ttu-id="3d7a3-126">なし</span><span class="sxs-lookup"><span data-stu-id="3d7a3-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d7a3-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d7a3-127">JSON Representation</span></span>
<span data-ttu-id="3d7a3-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d7a3-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```





