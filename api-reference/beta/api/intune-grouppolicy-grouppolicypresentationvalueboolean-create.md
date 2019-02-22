---
title: grouppolicypresentationvalueboolean の作成
description: 新しい grouppolicypresentationvalueboolean オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3b724865700daadc2c52ab5fa4c08e1e0ec690c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155441"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="dc65f-103">grouppolicypresentationvalueboolean の作成</span><span class="sxs-lookup"><span data-stu-id="dc65f-103">Create groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="dc65f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc65f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc65f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc65f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc65f-106">新しい[grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc65f-106">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc65f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc65f-107">Prerequisites</span></span>
<span data-ttu-id="dc65f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc65f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc65f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc65f-110">Permission type</span></span>|<span data-ttu-id="dc65f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc65f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc65f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc65f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc65f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc65f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc65f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc65f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc65f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc65f-115">Not supported.</span></span>|
|<span data-ttu-id="dc65f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc65f-116">Application</span></span>|<span data-ttu-id="dc65f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc65f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc65f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc65f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="dc65f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc65f-119">Request headers</span></span>
|<span data-ttu-id="dc65f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc65f-120">Header</span></span>|<span data-ttu-id="dc65f-121">値</span><span class="sxs-lookup"><span data-stu-id="dc65f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc65f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc65f-122">Authorization</span></span>|<span data-ttu-id="dc65f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dc65f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc65f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dc65f-124">Accept</span></span>|<span data-ttu-id="dc65f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc65f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc65f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc65f-126">Request body</span></span>
<span data-ttu-id="dc65f-127">要求本文で、grouppolicypresentationvalueboolean オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc65f-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="dc65f-128">次の表に、grouppolicypresentationvalueboolean の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dc65f-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="dc65f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc65f-129">Property</span></span>|<span data-ttu-id="dc65f-130">型</span><span class="sxs-lookup"><span data-stu-id="dc65f-130">Type</span></span>|<span data-ttu-id="dc65f-131">説明</span><span class="sxs-lookup"><span data-stu-id="dc65f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc65f-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc65f-132">lastModifiedDateTime</span></span>|<span data-ttu-id="dc65f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc65f-133">DateTimeOffset</span></span>|<span data-ttu-id="dc65f-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="dc65f-134">The date and time the object was last modified.</span></span> <span data-ttu-id="dc65f-135">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="dc65f-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="dc65f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc65f-136">createdDateTime</span></span>|<span data-ttu-id="dc65f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc65f-137">DateTimeOffset</span></span>|<span data-ttu-id="dc65f-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="dc65f-138">The date and time the object was created.</span></span> <span data-ttu-id="dc65f-139">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="dc65f-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="dc65f-140">id</span><span class="sxs-lookup"><span data-stu-id="dc65f-140">id</span></span>|<span data-ttu-id="dc65f-141">String</span><span class="sxs-lookup"><span data-stu-id="dc65f-141">String</span></span>|<span data-ttu-id="dc65f-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dc65f-142">Key of the entity.</span></span> <span data-ttu-id="dc65f-143">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="dc65f-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="dc65f-144">value</span><span class="sxs-lookup"><span data-stu-id="dc65f-144">value</span></span>|<span data-ttu-id="dc65f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc65f-145">Boolean</span></span>|<span data-ttu-id="dc65f-146">関連付けられたプレゼンテーションのブール値。</span><span class="sxs-lookup"><span data-stu-id="dc65f-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="dc65f-147">応答</span><span class="sxs-lookup"><span data-stu-id="dc65f-147">Response</span></span>
<span data-ttu-id="dc65f-148">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc65f-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc65f-149">例</span><span class="sxs-lookup"><span data-stu-id="dc65f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc65f-150">要求</span><span class="sxs-lookup"><span data-stu-id="dc65f-150">Request</span></span>
<span data-ttu-id="dc65f-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc65f-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="dc65f-152">応答</span><span class="sxs-lookup"><span data-stu-id="dc65f-152">Response</span></span>
<span data-ttu-id="dc65f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc65f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "be61344f-344f-be61-4f34-61be4f3461be",
  "value": true
}
```




