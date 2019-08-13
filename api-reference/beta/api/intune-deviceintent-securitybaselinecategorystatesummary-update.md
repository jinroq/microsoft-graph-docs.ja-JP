---
title: SecurityBaselineCategoryStateSummary の更新
description: SecurityBaselineCategoryStateSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67a7211a65fcd7d88e8245e7fd7aba641e655fd6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349167"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="a8877-103">SecurityBaselineCategoryStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a8877-103">Update securityBaselineCategoryStateSummary</span></span>

> <span data-ttu-id="a8877-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8877-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8877-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8877-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8877-106">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a8877-106">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8877-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a8877-107">Prerequisites</span></span>
<span data-ttu-id="a8877-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8877-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8877-110">Permission type</span></span>|<span data-ttu-id="a8877-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8877-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8877-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8877-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8877-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8877-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8877-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8877-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8877-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8877-115">Not supported.</span></span>|
|<span data-ttu-id="a8877-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8877-116">Application</span></span>|<span data-ttu-id="a8877-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8877-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8877-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8877-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a8877-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8877-119">Request headers</span></span>
|<span data-ttu-id="a8877-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8877-120">Header</span></span>|<span data-ttu-id="a8877-121">値</span><span class="sxs-lookup"><span data-stu-id="a8877-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8877-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8877-122">Authorization</span></span>|<span data-ttu-id="a8877-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8877-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8877-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a8877-124">Accept</span></span>|<span data-ttu-id="a8877-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8877-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8877-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8877-126">Request body</span></span>
<span data-ttu-id="a8877-127">要求本文で、 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8877-127">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="a8877-128">次の表に、 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a8877-128">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="a8877-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8877-129">Property</span></span>|<span data-ttu-id="a8877-130">型</span><span class="sxs-lookup"><span data-stu-id="a8877-130">Type</span></span>|<span data-ttu-id="a8877-131">説明</span><span class="sxs-lookup"><span data-stu-id="a8877-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8877-132">id</span><span class="sxs-lookup"><span data-stu-id="a8877-132">id</span></span>|<span data-ttu-id="a8877-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a8877-133">String</span></span>|<span data-ttu-id="a8877-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a8877-134">Unique identifier of the entity.</span></span> <span data-ttu-id="a8877-135">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a8877-135">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a8877-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="a8877-136">secureCount</span></span>|<span data-ttu-id="a8877-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a8877-137">Int32</span></span>|<span data-ttu-id="a8877-138">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されたデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a8877-138">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a8877-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="a8877-139">notSecureCount</span></span>|<span data-ttu-id="a8877-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a8877-140">Int32</span></span>|<span data-ttu-id="a8877-141">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a8877-141">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a8877-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="a8877-142">unknownCount</span></span>|<span data-ttu-id="a8877-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a8877-143">Int32</span></span>|<span data-ttu-id="a8877-144">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a8877-144">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a8877-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="a8877-145">errorCount</span></span>|<span data-ttu-id="a8877-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a8877-146">Int32</span></span>|<span data-ttu-id="a8877-147">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承されたエラーデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a8877-147">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a8877-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a8877-148">conflictCount</span></span>|<span data-ttu-id="a8877-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a8877-149">Int32</span></span>|<span data-ttu-id="a8877-150">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="a8877-150">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a8877-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a8877-151">notApplicableCount</span></span>|<span data-ttu-id="a8877-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a8877-152">Int32</span></span>|<span data-ttu-id="a8877-153">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された、適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a8877-153">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a8877-154">displayName</span><span class="sxs-lookup"><span data-stu-id="a8877-154">displayName</span></span>|<span data-ttu-id="a8877-155">String</span><span class="sxs-lookup"><span data-stu-id="a8877-155">String</span></span>|<span data-ttu-id="a8877-156">カテゴリ名</span><span class="sxs-lookup"><span data-stu-id="a8877-156">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="a8877-157">応答</span><span class="sxs-lookup"><span data-stu-id="a8877-157">Response</span></span>
<span data-ttu-id="a8877-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a8877-158">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8877-159">例</span><span class="sxs-lookup"><span data-stu-id="a8877-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8877-160">要求</span><span class="sxs-lookup"><span data-stu-id="a8877-160">Request</span></span>
<span data-ttu-id="a8877-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a8877-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a8877-162">応答</span><span class="sxs-lookup"><span data-stu-id="a8877-162">Response</span></span>
<span data-ttu-id="a8877-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a8877-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```






