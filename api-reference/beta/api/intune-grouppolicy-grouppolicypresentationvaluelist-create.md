---
title: grouppolicypresentationvaluelist の作成
description: 新しい grouppolicypresentationvaluelist オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a96c49817637e951f11b94e8dc2381df513c9a2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964872"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="f3894-103">grouppolicypresentationvaluelist の作成</span><span class="sxs-lookup"><span data-stu-id="f3894-103">Create groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="f3894-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3894-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3894-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3894-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3894-106">新しい[grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f3894-106">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3894-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3894-107">Prerequisites</span></span>
<span data-ttu-id="f3894-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3894-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3894-110">Permission type</span></span>|<span data-ttu-id="f3894-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3894-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3894-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3894-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3894-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3894-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f3894-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3894-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3894-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3894-115">Not supported.</span></span>|
|<span data-ttu-id="f3894-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3894-116">Application</span></span>|<span data-ttu-id="f3894-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3894-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3894-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3894-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="f3894-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3894-119">Request headers</span></span>
|<span data-ttu-id="f3894-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3894-120">Header</span></span>|<span data-ttu-id="f3894-121">値</span><span class="sxs-lookup"><span data-stu-id="f3894-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3894-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3894-122">Authorization</span></span>|<span data-ttu-id="f3894-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3894-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3894-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f3894-124">Accept</span></span>|<span data-ttu-id="f3894-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3894-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3894-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3894-126">Request body</span></span>
<span data-ttu-id="f3894-127">要求本文で、grouppolicypresentationvaluelist オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3894-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="f3894-128">次の表に、grouppolicypresentationvaluelist の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3894-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="f3894-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3894-129">Property</span></span>|<span data-ttu-id="f3894-130">型</span><span class="sxs-lookup"><span data-stu-id="f3894-130">Type</span></span>|<span data-ttu-id="f3894-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3894-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3894-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3894-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f3894-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3894-133">DateTimeOffset</span></span>|<span data-ttu-id="f3894-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f3894-134">The date and time the object was last modified.</span></span> <span data-ttu-id="f3894-135">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f3894-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f3894-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3894-136">createdDateTime</span></span>|<span data-ttu-id="f3894-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3894-137">DateTimeOffset</span></span>|<span data-ttu-id="f3894-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f3894-138">The date and time the object was created.</span></span> <span data-ttu-id="f3894-139">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f3894-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f3894-140">id</span><span class="sxs-lookup"><span data-stu-id="f3894-140">id</span></span>|<span data-ttu-id="f3894-141">String</span><span class="sxs-lookup"><span data-stu-id="f3894-141">String</span></span>|<span data-ttu-id="f3894-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3894-142">Key of the entity.</span></span> <span data-ttu-id="f3894-143">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f3894-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f3894-144">values</span><span class="sxs-lookup"><span data-stu-id="f3894-144">values</span></span>|<span data-ttu-id="f3894-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f3894-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f3894-146">関連付けられているプレゼンテーションのペアのリスト。</span><span class="sxs-lookup"><span data-stu-id="f3894-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="f3894-147">応答</span><span class="sxs-lookup"><span data-stu-id="f3894-147">Response</span></span>
<span data-ttu-id="f3894-148">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3894-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3894-149">例</span><span class="sxs-lookup"><span data-stu-id="f3894-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3894-150">要求</span><span class="sxs-lookup"><span data-stu-id="f3894-150">Request</span></span>
<span data-ttu-id="f3894-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3894-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f3894-152">応答</span><span class="sxs-lookup"><span data-stu-id="f3894-152">Response</span></span>
<span data-ttu-id="f3894-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3894-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




