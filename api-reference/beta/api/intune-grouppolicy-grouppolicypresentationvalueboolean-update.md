---
title: grouppolicypresentationvalueboolean の更新
description: grouppolicypresentationvalueboolean オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1a249347f3c1e7717558e9872ad0524e278cd56
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970066"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="f0ad0-103">grouppolicypresentationvalueboolean の更新</span><span class="sxs-lookup"><span data-stu-id="f0ad0-103">Update groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="f0ad0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0ad0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0ad0-106">[grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-106">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0ad0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f0ad0-107">Prerequisites</span></span>
<span data-ttu-id="f0ad0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0ad0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0ad0-110">Permission type</span></span>|<span data-ttu-id="f0ad0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0ad0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0ad0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0ad0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0ad0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0ad0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0ad0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0ad0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0ad0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-115">Not supported.</span></span>|
|<span data-ttu-id="f0ad0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0ad0-116">Application</span></span>|<span data-ttu-id="f0ad0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0ad0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0ad0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="f0ad0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0ad0-119">Request headers</span></span>
|<span data-ttu-id="f0ad0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0ad0-120">Header</span></span>|<span data-ttu-id="f0ad0-121">値</span><span class="sxs-lookup"><span data-stu-id="f0ad0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0ad0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0ad0-122">Authorization</span></span>|<span data-ttu-id="f0ad0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0ad0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f0ad0-124">Accept</span></span>|<span data-ttu-id="f0ad0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0ad0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0ad0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0ad0-126">Request body</span></span>
<span data-ttu-id="f0ad0-127">要求本文で、 [grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="f0ad0-128">次の表に、 [grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="f0ad0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0ad0-129">Property</span></span>|<span data-ttu-id="f0ad0-130">型</span><span class="sxs-lookup"><span data-stu-id="f0ad0-130">Type</span></span>|<span data-ttu-id="f0ad0-131">説明</span><span class="sxs-lookup"><span data-stu-id="f0ad0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0ad0-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0ad0-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f0ad0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0ad0-133">DateTimeOffset</span></span>|<span data-ttu-id="f0ad0-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-134">The date and time the object was last modified.</span></span> <span data-ttu-id="f0ad0-135">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f0ad0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0ad0-136">createdDateTime</span></span>|<span data-ttu-id="f0ad0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0ad0-137">DateTimeOffset</span></span>|<span data-ttu-id="f0ad0-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-138">The date and time the object was created.</span></span> <span data-ttu-id="f0ad0-139">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f0ad0-140">id</span><span class="sxs-lookup"><span data-stu-id="f0ad0-140">id</span></span>|<span data-ttu-id="f0ad0-141">String</span><span class="sxs-lookup"><span data-stu-id="f0ad0-141">String</span></span>|<span data-ttu-id="f0ad0-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-142">Key of the entity.</span></span> <span data-ttu-id="f0ad0-143">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f0ad0-144">value</span><span class="sxs-lookup"><span data-stu-id="f0ad0-144">value</span></span>|<span data-ttu-id="f0ad0-145">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f0ad0-145">Boolean</span></span>|<span data-ttu-id="f0ad0-146">関連付けられたプレゼンテーションのブール値。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="f0ad0-147">応答</span><span class="sxs-lookup"><span data-stu-id="f0ad0-147">Response</span></span>
<span data-ttu-id="f0ad0-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0ad0-149">例</span><span class="sxs-lookup"><span data-stu-id="f0ad0-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0ad0-150">要求</span><span class="sxs-lookup"><span data-stu-id="f0ad0-150">Request</span></span>
<span data-ttu-id="f0ad0-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="f0ad0-152">応答</span><span class="sxs-lookup"><span data-stu-id="f0ad0-152">Response</span></span>
<span data-ttu-id="f0ad0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0ad0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




