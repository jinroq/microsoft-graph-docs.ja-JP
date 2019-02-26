---
title: groupPolicyPresentationValueDecimal の更新
description: groupPolicyPresentationValueDecimal オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39d9fe3e0a6d9e54d951f1ee8bcf80f53ee1575f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152347"
---
# <a name="update-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="8a8db-103">groupPolicyPresentationValueDecimal の更新</span><span class="sxs-lookup"><span data-stu-id="8a8db-103">Update groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="8a8db-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a8db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a8db-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a8db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a8db-106">[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8a8db-106">Update the properties of a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a8db-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a8db-107">Prerequisites</span></span>
<span data-ttu-id="8a8db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a8db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8a8db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a8db-110">Permission type</span></span>|<span data-ttu-id="8a8db-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a8db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a8db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a8db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a8db-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a8db-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8a8db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a8db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a8db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a8db-115">Not supported.</span></span>|
|<span data-ttu-id="8a8db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a8db-116">Application</span></span>|<span data-ttu-id="8a8db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a8db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a8db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a8db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="8a8db-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a8db-119">Request headers</span></span>
|<span data-ttu-id="8a8db-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a8db-120">Header</span></span>|<span data-ttu-id="8a8db-121">値</span><span class="sxs-lookup"><span data-stu-id="8a8db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a8db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a8db-122">Authorization</span></span>|<span data-ttu-id="8a8db-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8a8db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a8db-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8a8db-124">Accept</span></span>|<span data-ttu-id="8a8db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a8db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a8db-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a8db-126">Request body</span></span>
<span data-ttu-id="8a8db-127">要求本文で、 [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a8db-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

<span data-ttu-id="8a8db-128">次の表に、 [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8a8db-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span></span>

|<span data-ttu-id="8a8db-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a8db-129">Property</span></span>|<span data-ttu-id="8a8db-130">型</span><span class="sxs-lookup"><span data-stu-id="8a8db-130">Type</span></span>|<span data-ttu-id="8a8db-131">説明</span><span class="sxs-lookup"><span data-stu-id="8a8db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a8db-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a8db-132">lastModifiedDateTime</span></span>|<span data-ttu-id="8a8db-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a8db-133">DateTimeOffset</span></span>|<span data-ttu-id="8a8db-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8a8db-134">The date and time the object was last modified.</span></span> <span data-ttu-id="8a8db-135">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8a8db-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8a8db-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a8db-136">createdDateTime</span></span>|<span data-ttu-id="8a8db-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a8db-137">DateTimeOffset</span></span>|<span data-ttu-id="8a8db-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8a8db-138">The date and time the object was created.</span></span> <span data-ttu-id="8a8db-139">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8a8db-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8a8db-140">id</span><span class="sxs-lookup"><span data-stu-id="8a8db-140">id</span></span>|<span data-ttu-id="8a8db-141">String</span><span class="sxs-lookup"><span data-stu-id="8a8db-141">String</span></span>|<span data-ttu-id="8a8db-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8a8db-142">Key of the entity.</span></span> <span data-ttu-id="8a8db-143">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8a8db-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8a8db-144">value</span><span class="sxs-lookup"><span data-stu-id="8a8db-144">value</span></span>|<span data-ttu-id="8a8db-145">Int64</span><span class="sxs-lookup"><span data-stu-id="8a8db-145">Int64</span></span>|<span data-ttu-id="8a8db-146">関連付けられたプレゼンテーションの符号なし整数値。</span><span class="sxs-lookup"><span data-stu-id="8a8db-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="8a8db-147">応答</span><span class="sxs-lookup"><span data-stu-id="8a8db-147">Response</span></span>
<span data-ttu-id="8a8db-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8a8db-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a8db-149">例</span><span class="sxs-lookup"><span data-stu-id="8a8db-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a8db-150">要求</span><span class="sxs-lookup"><span data-stu-id="8a8db-150">Request</span></span>
<span data-ttu-id="8a8db-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a8db-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="8a8db-152">応答</span><span class="sxs-lookup"><span data-stu-id="8a8db-152">Response</span></span>
<span data-ttu-id="8a8db-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a8db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




