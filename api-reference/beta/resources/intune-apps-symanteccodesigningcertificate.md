---
title: symantecCodeSigningCertificate リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 979502f51674b32f10627762d08d8216a466dff9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357240"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="ae083-103">symantecCodeSigningCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae083-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="ae083-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae083-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae083-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae083-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae083-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae083-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae083-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ae083-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="ae083-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae083-108">Methods</span></span>
|<span data-ttu-id="ae083-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae083-109">Method</span></span>|<span data-ttu-id="ae083-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ae083-110">Return Type</span></span>|<span data-ttu-id="ae083-111">説明</span><span class="sxs-lookup"><span data-stu-id="ae083-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae083-112">SymantecCodeSigningCertificate を取得します。</span><span class="sxs-lookup"><span data-stu-id="ae083-112">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="ae083-113">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="ae083-113">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="ae083-114">[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae083-114">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="ae083-115">SymantecCodeSigningCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="ae083-115">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="ae083-116">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="ae083-116">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="ae083-117">[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae083-117">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae083-118">Properties</span><span class="sxs-lookup"><span data-stu-id="ae083-118">Properties</span></span>
|<span data-ttu-id="ae083-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae083-119">Property</span></span>|<span data-ttu-id="ae083-120">種類</span><span class="sxs-lookup"><span data-stu-id="ae083-120">Type</span></span>|<span data-ttu-id="ae083-121">説明</span><span class="sxs-lookup"><span data-stu-id="ae083-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae083-122">ID</span><span class="sxs-lookup"><span data-stu-id="ae083-122">id</span></span>|<span data-ttu-id="ae083-123">String</span><span class="sxs-lookup"><span data-stu-id="ae083-123">String</span></span>|<span data-ttu-id="ae083-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae083-124">The key of the entity.</span></span>|
|<span data-ttu-id="ae083-125">content</span><span class="sxs-lookup"><span data-stu-id="ae083-125">content</span></span>|<span data-ttu-id="ae083-126">Binary</span><span class="sxs-lookup"><span data-stu-id="ae083-126">Binary</span></span>|<span data-ttu-id="ae083-127">生データの形式で Windows のシマンテック社のコード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="ae083-127">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="ae083-128">status</span><span class="sxs-lookup"><span data-stu-id="ae083-128">status</span></span>|[<span data-ttu-id="ae083-129">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="ae083-129">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="ae083-130">証明書の状態は、準備または準備されていません。</span><span class="sxs-lookup"><span data-stu-id="ae083-130">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="ae083-131">使用可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="ae083-131">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="ae083-132">password</span><span class="sxs-lookup"><span data-stu-id="ae083-132">password</span></span>|<span data-ttu-id="ae083-133">String</span><span class="sxs-lookup"><span data-stu-id="ae083-133">String</span></span>|<span data-ttu-id="ae083-134">.Pfx ファイルに必要なパスワードです。</span><span class="sxs-lookup"><span data-stu-id="ae083-134">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="ae083-135">subjectName</span><span class="sxs-lookup"><span data-stu-id="ae083-135">subjectName</span></span>|<span data-ttu-id="ae083-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ae083-136">String</span></span>|<span data-ttu-id="ae083-137">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="ae083-137">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="ae083-138">subject</span><span class="sxs-lookup"><span data-stu-id="ae083-138">subject</span></span>|<span data-ttu-id="ae083-139">String</span><span class="sxs-lookup"><span data-stu-id="ae083-139">String</span></span>|<span data-ttu-id="ae083-140">証明書のサブジェクト値。</span><span class="sxs-lookup"><span data-stu-id="ae083-140">The Subject value for the cert.</span></span>|
|<span data-ttu-id="ae083-141">issuerName</span><span class="sxs-lookup"><span data-stu-id="ae083-141">issuerName</span></span>|<span data-ttu-id="ae083-142">String</span><span class="sxs-lookup"><span data-stu-id="ae083-142">String</span></span>|<span data-ttu-id="ae083-143">証明書の発行者の名前です。</span><span class="sxs-lookup"><span data-stu-id="ae083-143">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="ae083-144">発行者</span><span class="sxs-lookup"><span data-stu-id="ae083-144">issuer</span></span>|<span data-ttu-id="ae083-145">String</span><span class="sxs-lookup"><span data-stu-id="ae083-145">String</span></span>|<span data-ttu-id="ae083-146">証明書の発行者の値です。</span><span class="sxs-lookup"><span data-stu-id="ae083-146">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="ae083-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ae083-147">expirationDateTime</span></span>|<span data-ttu-id="ae083-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae083-148">DateTimeOffset</span></span>|<span data-ttu-id="ae083-149">証明書の有効期限日です。</span><span class="sxs-lookup"><span data-stu-id="ae083-149">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="ae083-150">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="ae083-150">uploadDateTime</span></span>|<span data-ttu-id="ae083-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae083-151">DateTimeOffset</span></span>|<span data-ttu-id="ae083-152">シマンテック社の証明書とコード署名証明書の種類です。</span><span class="sxs-lookup"><span data-stu-id="ae083-152">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae083-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae083-153">Relationships</span></span>
<span data-ttu-id="ae083-154">なし</span><span class="sxs-lookup"><span data-stu-id="ae083-154">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae083-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae083-155">JSON Representation</span></span>
<span data-ttu-id="ae083-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae083-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```





