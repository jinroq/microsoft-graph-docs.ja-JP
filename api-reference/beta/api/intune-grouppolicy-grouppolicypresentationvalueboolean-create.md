---
title: GroupPolicyPresentationValueBoolean を作成します。
description: 新しい groupPolicyPresentationValueBoolean オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcf9a25b882bc9b952ed2b052e7b096ac45223dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430253"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="3576b-103">GroupPolicyPresentationValueBoolean を作成します。</span><span class="sxs-lookup"><span data-stu-id="3576b-103">Create groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="3576b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3576b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3576b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3576b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3576b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3576b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3576b-107">新しい[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3576b-107">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3576b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3576b-108">Prerequisites</span></span>
<span data-ttu-id="3576b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3576b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3576b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3576b-111">Permission type</span></span>|<span data-ttu-id="3576b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3576b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3576b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3576b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3576b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3576b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3576b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3576b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3576b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3576b-116">Not supported.</span></span>|
|<span data-ttu-id="3576b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3576b-117">Application</span></span>|<span data-ttu-id="3576b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3576b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3576b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3576b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="3576b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3576b-120">Request headers</span></span>
|<span data-ttu-id="3576b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3576b-121">Header</span></span>|<span data-ttu-id="3576b-122">値</span><span class="sxs-lookup"><span data-stu-id="3576b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3576b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3576b-123">Authorization</span></span>|<span data-ttu-id="3576b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3576b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3576b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3576b-125">Accept</span></span>|<span data-ttu-id="3576b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3576b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3576b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3576b-127">Request body</span></span>
<span data-ttu-id="3576b-128">要求の本文に groupPolicyPresentationValueBoolean オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3576b-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="3576b-129">次の表は、groupPolicyPresentationValueBoolean を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3576b-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="3576b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3576b-130">Property</span></span>|<span data-ttu-id="3576b-131">型</span><span class="sxs-lookup"><span data-stu-id="3576b-131">Type</span></span>|<span data-ttu-id="3576b-132">説明</span><span class="sxs-lookup"><span data-stu-id="3576b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3576b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3576b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3576b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3576b-134">DateTimeOffset</span></span>|<span data-ttu-id="3576b-135">日付と時刻オブジェクトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="3576b-135">The date and time the object was last modified.</span></span> <span data-ttu-id="3576b-136">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3576b-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3576b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3576b-137">createdDateTime</span></span>|<span data-ttu-id="3576b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3576b-138">DateTimeOffset</span></span>|<span data-ttu-id="3576b-139">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3576b-139">The date and time the object was created.</span></span> <span data-ttu-id="3576b-140">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3576b-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3576b-141">id</span><span class="sxs-lookup"><span data-stu-id="3576b-141">id</span></span>|<span data-ttu-id="3576b-142">String</span><span class="sxs-lookup"><span data-stu-id="3576b-142">String</span></span>|<span data-ttu-id="3576b-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3576b-143">Key of the entity.</span></span> <span data-ttu-id="3576b-144">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3576b-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3576b-145">value</span><span class="sxs-lookup"><span data-stu-id="3576b-145">value</span></span>|<span data-ttu-id="3576b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3576b-146">Boolean</span></span>|<span data-ttu-id="3576b-147">関連付けられているプレゼンテーション用のブール値です。</span><span class="sxs-lookup"><span data-stu-id="3576b-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="3576b-148">応答</span><span class="sxs-lookup"><span data-stu-id="3576b-148">Response</span></span>
<span data-ttu-id="3576b-149">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3576b-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3576b-150">例</span><span class="sxs-lookup"><span data-stu-id="3576b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3576b-151">要求</span><span class="sxs-lookup"><span data-stu-id="3576b-151">Request</span></span>
<span data-ttu-id="3576b-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3576b-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="3576b-153">応答</span><span class="sxs-lookup"><span data-stu-id="3576b-153">Response</span></span>
<span data-ttu-id="3576b-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3576b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




