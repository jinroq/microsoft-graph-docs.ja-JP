---
title: GroupPolicyPresentationValueDecimal の更新
description: GroupPolicyPresentationValueDecimal オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21dac69bc9cfe37cce3f4e392dfee766ab3fe600
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354570"
---
# <a name="update-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="cfa4b-103">GroupPolicyPresentationValueDecimal の更新</span><span class="sxs-lookup"><span data-stu-id="cfa4b-103">Update groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="cfa4b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfa4b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfa4b-106">[GroupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-106">Update the properties of a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfa4b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cfa4b-107">Prerequisites</span></span>
<span data-ttu-id="cfa4b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfa4b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfa4b-110">Permission type</span></span>|<span data-ttu-id="cfa4b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfa4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfa4b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfa4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfa4b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfa4b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cfa4b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfa4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfa4b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-115">Not supported.</span></span>|
|<span data-ttu-id="cfa4b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfa4b-116">Application</span></span>|<span data-ttu-id="cfa4b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfa4b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfa4b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfa4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="cfa4b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfa4b-119">Request headers</span></span>
|<span data-ttu-id="cfa4b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfa4b-120">Header</span></span>|<span data-ttu-id="cfa4b-121">値</span><span class="sxs-lookup"><span data-stu-id="cfa4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfa4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfa4b-122">Authorization</span></span>|<span data-ttu-id="cfa4b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfa4b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cfa4b-124">Accept</span></span>|<span data-ttu-id="cfa4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfa4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfa4b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfa4b-126">Request body</span></span>
<span data-ttu-id="cfa4b-127">要求本文で、 [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

<span data-ttu-id="cfa4b-128">次の表に、 [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span></span>

|<span data-ttu-id="cfa4b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfa4b-129">Property</span></span>|<span data-ttu-id="cfa4b-130">型</span><span class="sxs-lookup"><span data-stu-id="cfa4b-130">Type</span></span>|<span data-ttu-id="cfa4b-131">説明</span><span class="sxs-lookup"><span data-stu-id="cfa4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfa4b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfa4b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="cfa4b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfa4b-133">DateTimeOffset</span></span>|<span data-ttu-id="cfa4b-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-134">The date and time the object was last modified.</span></span> <span data-ttu-id="cfa4b-135">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cfa4b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfa4b-136">createdDateTime</span></span>|<span data-ttu-id="cfa4b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfa4b-137">DateTimeOffset</span></span>|<span data-ttu-id="cfa4b-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-138">The date and time the object was created.</span></span> <span data-ttu-id="cfa4b-139">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cfa4b-140">id</span><span class="sxs-lookup"><span data-stu-id="cfa4b-140">id</span></span>|<span data-ttu-id="cfa4b-141">String</span><span class="sxs-lookup"><span data-stu-id="cfa4b-141">String</span></span>|<span data-ttu-id="cfa4b-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-142">Key of the entity.</span></span> <span data-ttu-id="cfa4b-143">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cfa4b-144">value</span><span class="sxs-lookup"><span data-stu-id="cfa4b-144">value</span></span>|<span data-ttu-id="cfa4b-145">Int64</span><span class="sxs-lookup"><span data-stu-id="cfa4b-145">Int64</span></span>|<span data-ttu-id="cfa4b-146">関連付けられたプレゼンテーションの符号なし整数値。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="cfa4b-147">応答</span><span class="sxs-lookup"><span data-stu-id="cfa4b-147">Response</span></span>
<span data-ttu-id="cfa4b-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfa4b-149">例</span><span class="sxs-lookup"><span data-stu-id="cfa4b-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfa4b-150">要求</span><span class="sxs-lookup"><span data-stu-id="cfa4b-150">Request</span></span>
<span data-ttu-id="cfa4b-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="cfa4b-152">応答</span><span class="sxs-lookup"><span data-stu-id="cfa4b-152">Response</span></span>
<span data-ttu-id="cfa4b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cfa4b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```






