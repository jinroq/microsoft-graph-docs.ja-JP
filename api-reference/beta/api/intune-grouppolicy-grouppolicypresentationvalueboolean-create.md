---
title: GroupPolicyPresentationValueBoolean の作成
description: 新しい groupPolicyPresentationValueBoolean オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93499dfaa852b1fef4d465259bd7a6c9ddedcfff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357587"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="1d262-103">GroupPolicyPresentationValueBoolean の作成</span><span class="sxs-lookup"><span data-stu-id="1d262-103">Create groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="1d262-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d262-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d262-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d262-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d262-106">新しい[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1d262-106">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d262-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1d262-107">Prerequisites</span></span>
<span data-ttu-id="1d262-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d262-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d262-110">Permission type</span></span>|<span data-ttu-id="1d262-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d262-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d262-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d262-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d262-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d262-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d262-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d262-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d262-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d262-115">Not supported.</span></span>|
|<span data-ttu-id="1d262-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d262-116">Application</span></span>|<span data-ttu-id="1d262-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d262-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d262-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d262-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="1d262-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d262-119">Request headers</span></span>
|<span data-ttu-id="1d262-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d262-120">Header</span></span>|<span data-ttu-id="1d262-121">値</span><span class="sxs-lookup"><span data-stu-id="1d262-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d262-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d262-122">Authorization</span></span>|<span data-ttu-id="1d262-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d262-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d262-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1d262-124">Accept</span></span>|<span data-ttu-id="1d262-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d262-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d262-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d262-126">Request body</span></span>
<span data-ttu-id="1d262-127">要求本文で、groupPolicyPresentationValueBoolean オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d262-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="1d262-128">次の表に、groupPolicyPresentationValueBoolean の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1d262-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="1d262-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d262-129">Property</span></span>|<span data-ttu-id="1d262-130">型</span><span class="sxs-lookup"><span data-stu-id="1d262-130">Type</span></span>|<span data-ttu-id="1d262-131">説明</span><span class="sxs-lookup"><span data-stu-id="1d262-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d262-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d262-132">lastModifiedDateTime</span></span>|<span data-ttu-id="1d262-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d262-133">DateTimeOffset</span></span>|<span data-ttu-id="1d262-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="1d262-134">The date and time the object was last modified.</span></span> <span data-ttu-id="1d262-135">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1d262-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1d262-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d262-136">createdDateTime</span></span>|<span data-ttu-id="1d262-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d262-137">DateTimeOffset</span></span>|<span data-ttu-id="1d262-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="1d262-138">The date and time the object was created.</span></span> <span data-ttu-id="1d262-139">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1d262-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1d262-140">id</span><span class="sxs-lookup"><span data-stu-id="1d262-140">id</span></span>|<span data-ttu-id="1d262-141">String</span><span class="sxs-lookup"><span data-stu-id="1d262-141">String</span></span>|<span data-ttu-id="1d262-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1d262-142">Key of the entity.</span></span> <span data-ttu-id="1d262-143">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1d262-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1d262-144">value</span><span class="sxs-lookup"><span data-stu-id="1d262-144">value</span></span>|<span data-ttu-id="1d262-145">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1d262-145">Boolean</span></span>|<span data-ttu-id="1d262-146">関連付けられたプレゼンテーションのブール値。</span><span class="sxs-lookup"><span data-stu-id="1d262-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="1d262-147">応答</span><span class="sxs-lookup"><span data-stu-id="1d262-147">Response</span></span>
<span data-ttu-id="1d262-148">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d262-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d262-149">例</span><span class="sxs-lookup"><span data-stu-id="1d262-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d262-150">要求</span><span class="sxs-lookup"><span data-stu-id="1d262-150">Request</span></span>
<span data-ttu-id="1d262-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d262-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="1d262-152">応答</span><span class="sxs-lookup"><span data-stu-id="1d262-152">Response</span></span>
<span data-ttu-id="1d262-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d262-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






