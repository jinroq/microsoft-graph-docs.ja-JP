---
title: GroupPolicyPresentationValueMultiText を更新します。
description: GroupPolicyPresentationValueMultiText オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 030f1a422106eeda59e77f06ce37d60688744b53
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430529"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="8a289-103">GroupPolicyPresentationValueMultiText を更新します。</span><span class="sxs-lookup"><span data-stu-id="8a289-103">Update groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="8a289-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a289-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8a289-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a289-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a289-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a289-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a289-107">[GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8a289-107">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a289-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a289-108">Prerequisites</span></span>
<span data-ttu-id="8a289-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a289-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8a289-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a289-111">Permission type</span></span>|<span data-ttu-id="8a289-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a289-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a289-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a289-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a289-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a289-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8a289-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a289-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a289-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a289-116">Not supported.</span></span>|
|<span data-ttu-id="8a289-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a289-117">Application</span></span>|<span data-ttu-id="8a289-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a289-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a289-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a289-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="8a289-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a289-120">Request headers</span></span>
|<span data-ttu-id="8a289-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a289-121">Header</span></span>|<span data-ttu-id="8a289-122">値</span><span class="sxs-lookup"><span data-stu-id="8a289-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a289-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a289-123">Authorization</span></span>|<span data-ttu-id="8a289-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8a289-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a289-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a289-125">Accept</span></span>|<span data-ttu-id="8a289-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a289-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a289-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a289-127">Request body</span></span>
<span data-ttu-id="8a289-128">要求の本文に[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a289-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="8a289-129">[GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="8a289-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="8a289-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a289-130">Property</span></span>|<span data-ttu-id="8a289-131">型</span><span class="sxs-lookup"><span data-stu-id="8a289-131">Type</span></span>|<span data-ttu-id="8a289-132">説明</span><span class="sxs-lookup"><span data-stu-id="8a289-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a289-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a289-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8a289-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a289-134">DateTimeOffset</span></span>|<span data-ttu-id="8a289-135">日付と時刻オブジェクトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="8a289-135">The date and time the object was last modified.</span></span> <span data-ttu-id="8a289-136">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8a289-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8a289-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a289-137">createdDateTime</span></span>|<span data-ttu-id="8a289-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a289-138">DateTimeOffset</span></span>|<span data-ttu-id="8a289-139">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8a289-139">The date and time the object was created.</span></span> <span data-ttu-id="8a289-140">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8a289-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8a289-141">id</span><span class="sxs-lookup"><span data-stu-id="8a289-141">id</span></span>|<span data-ttu-id="8a289-142">String</span><span class="sxs-lookup"><span data-stu-id="8a289-142">String</span></span>|<span data-ttu-id="8a289-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8a289-143">Key of the entity.</span></span> <span data-ttu-id="8a289-144">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8a289-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8a289-145">values</span><span class="sxs-lookup"><span data-stu-id="8a289-145">values</span></span>|<span data-ttu-id="8a289-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8a289-146">String collection</span></span>|<span data-ttu-id="8a289-147">関連付けられているプレゼンテーションの空でない文字列のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8a289-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="8a289-148">応答</span><span class="sxs-lookup"><span data-stu-id="8a289-148">Response</span></span>
<span data-ttu-id="8a289-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8a289-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a289-150">例</span><span class="sxs-lookup"><span data-stu-id="8a289-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a289-151">要求</span><span class="sxs-lookup"><span data-stu-id="8a289-151">Request</span></span>
<span data-ttu-id="8a289-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a289-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8a289-153">応答</span><span class="sxs-lookup"><span data-stu-id="8a289-153">Response</span></span>
<span data-ttu-id="8a289-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a289-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```




