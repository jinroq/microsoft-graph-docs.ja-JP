---
title: securityBaselineStateSummary の更新
description: securityBaselineStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5ac7e4094f415af6b2922eaa03af663d0cf0572
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466204"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="0c9fd-103">securityBaselineStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="0c9fd-103">Update securityBaselineStateSummary</span></span>

> <span data-ttu-id="0c9fd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c9fd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c9fd-106">[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-106">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c9fd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c9fd-107">Prerequisites</span></span>
<span data-ttu-id="0c9fd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c9fd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c9fd-110">Permission type</span></span>|<span data-ttu-id="0c9fd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c9fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c9fd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c9fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c9fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c9fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c9fd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c9fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c9fd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-115">Not supported.</span></span>|
|<span data-ttu-id="0c9fd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c9fd-116">Application</span></span>|<span data-ttu-id="0c9fd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c9fd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c9fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="0c9fd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c9fd-119">Request headers</span></span>
|<span data-ttu-id="0c9fd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c9fd-120">Header</span></span>|<span data-ttu-id="0c9fd-121">値</span><span class="sxs-lookup"><span data-stu-id="0c9fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c9fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c9fd-122">Authorization</span></span>|<span data-ttu-id="0c9fd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c9fd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0c9fd-124">Accept</span></span>|<span data-ttu-id="0c9fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c9fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c9fd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c9fd-126">Request body</span></span>
<span data-ttu-id="0c9fd-127">要求本文で、 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-127">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="0c9fd-128">次の表に、 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-128">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="0c9fd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c9fd-129">Property</span></span>|<span data-ttu-id="0c9fd-130">型</span><span class="sxs-lookup"><span data-stu-id="0c9fd-130">Type</span></span>|<span data-ttu-id="0c9fd-131">説明</span><span class="sxs-lookup"><span data-stu-id="0c9fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c9fd-132">id</span><span class="sxs-lookup"><span data-stu-id="0c9fd-132">id</span></span>|<span data-ttu-id="0c9fd-133">String</span><span class="sxs-lookup"><span data-stu-id="0c9fd-133">String</span></span>|<span data-ttu-id="0c9fd-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0c9fd-135">secureCount</span><span class="sxs-lookup"><span data-stu-id="0c9fd-135">secureCount</span></span>|<span data-ttu-id="0c9fd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0c9fd-136">Int32</span></span>|<span data-ttu-id="0c9fd-137">セキュリティで保護されたデバイスの数</span><span class="sxs-lookup"><span data-stu-id="0c9fd-137">Number of secure devices</span></span>|
|<span data-ttu-id="0c9fd-138">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="0c9fd-138">notSecureCount</span></span>|<span data-ttu-id="0c9fd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0c9fd-139">Int32</span></span>|<span data-ttu-id="0c9fd-140">セキュリティで保護されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="0c9fd-140">Number of not secure devices</span></span>|
|<span data-ttu-id="0c9fd-141">unknownCount</span><span class="sxs-lookup"><span data-stu-id="0c9fd-141">unknownCount</span></span>|<span data-ttu-id="0c9fd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0c9fd-142">Int32</span></span>|<span data-ttu-id="0c9fd-143">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="0c9fd-143">Number of unknown devices</span></span>|
|<span data-ttu-id="0c9fd-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="0c9fd-144">errorCount</span></span>|<span data-ttu-id="0c9fd-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0c9fd-145">Int32</span></span>|<span data-ttu-id="0c9fd-146">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="0c9fd-146">Number of error devices</span></span>|
|<span data-ttu-id="0c9fd-147">conflictCount</span><span class="sxs-lookup"><span data-stu-id="0c9fd-147">conflictCount</span></span>|<span data-ttu-id="0c9fd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0c9fd-148">Int32</span></span>|<span data-ttu-id="0c9fd-149">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="0c9fd-149">Number of conflict devices</span></span>|
|<span data-ttu-id="0c9fd-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0c9fd-150">notApplicableCount</span></span>|<span data-ttu-id="0c9fd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0c9fd-151">Int32</span></span>|<span data-ttu-id="0c9fd-152">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="0c9fd-152">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="0c9fd-153">応答</span><span class="sxs-lookup"><span data-stu-id="0c9fd-153">Response</span></span>
<span data-ttu-id="0c9fd-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-154">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c9fd-155">例</span><span class="sxs-lookup"><span data-stu-id="0c9fd-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c9fd-156">要求</span><span class="sxs-lookup"><span data-stu-id="0c9fd-156">Request</span></span>
<span data-ttu-id="0c9fd-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

### <a name="response"></a><span data-ttu-id="0c9fd-158">応答</span><span class="sxs-lookup"><span data-stu-id="0c9fd-158">Response</span></span>
<span data-ttu-id="0c9fd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c9fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```





