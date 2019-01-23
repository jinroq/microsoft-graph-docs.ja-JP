---
title: GroupPolicyPresentationValueDecimal を更新します。
description: GroupPolicyPresentationValueDecimal オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 44f1472b9b8340fbda84251e671fab8d3196d1e8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431638"
---
# <a name="update-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="156f1-103">GroupPolicyPresentationValueDecimal を更新します。</span><span class="sxs-lookup"><span data-stu-id="156f1-103">Update groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="156f1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="156f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="156f1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="156f1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="156f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="156f1-107">[GroupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="156f1-107">Update the properties of a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="156f1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="156f1-108">Prerequisites</span></span>
<span data-ttu-id="156f1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="156f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="156f1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="156f1-111">Permission type</span></span>|<span data-ttu-id="156f1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="156f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="156f1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="156f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="156f1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="156f1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="156f1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="156f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="156f1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156f1-116">Not supported.</span></span>|
|<span data-ttu-id="156f1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="156f1-117">Application</span></span>|<span data-ttu-id="156f1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="156f1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="156f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="156f1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="156f1-120">Request headers</span></span>
|<span data-ttu-id="156f1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="156f1-121">Header</span></span>|<span data-ttu-id="156f1-122">値</span><span class="sxs-lookup"><span data-stu-id="156f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="156f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="156f1-123">Authorization</span></span>|<span data-ttu-id="156f1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="156f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="156f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="156f1-125">Accept</span></span>|<span data-ttu-id="156f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="156f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="156f1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="156f1-127">Request body</span></span>
<span data-ttu-id="156f1-128">要求の本文に[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="156f1-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

<span data-ttu-id="156f1-129">[GroupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="156f1-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span></span>

|<span data-ttu-id="156f1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="156f1-130">Property</span></span>|<span data-ttu-id="156f1-131">型</span><span class="sxs-lookup"><span data-stu-id="156f1-131">Type</span></span>|<span data-ttu-id="156f1-132">説明</span><span class="sxs-lookup"><span data-stu-id="156f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="156f1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="156f1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="156f1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156f1-134">DateTimeOffset</span></span>|<span data-ttu-id="156f1-135">日付と時刻オブジェクトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="156f1-135">The date and time the object was last modified.</span></span> <span data-ttu-id="156f1-136">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="156f1-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="156f1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="156f1-137">createdDateTime</span></span>|<span data-ttu-id="156f1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156f1-138">DateTimeOffset</span></span>|<span data-ttu-id="156f1-139">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="156f1-139">The date and time the object was created.</span></span> <span data-ttu-id="156f1-140">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="156f1-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="156f1-141">id</span><span class="sxs-lookup"><span data-stu-id="156f1-141">id</span></span>|<span data-ttu-id="156f1-142">String</span><span class="sxs-lookup"><span data-stu-id="156f1-142">String</span></span>|<span data-ttu-id="156f1-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="156f1-143">Key of the entity.</span></span> <span data-ttu-id="156f1-144">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="156f1-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="156f1-145">value</span><span class="sxs-lookup"><span data-stu-id="156f1-145">value</span></span>|<span data-ttu-id="156f1-146">Int64</span><span class="sxs-lookup"><span data-stu-id="156f1-146">Int64</span></span>|<span data-ttu-id="156f1-147">関連付けられているプレゼンテーションの符号なし整数値。</span><span class="sxs-lookup"><span data-stu-id="156f1-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="156f1-148">応答</span><span class="sxs-lookup"><span data-stu-id="156f1-148">Response</span></span>
<span data-ttu-id="156f1-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="156f1-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="156f1-150">例</span><span class="sxs-lookup"><span data-stu-id="156f1-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="156f1-151">要求</span><span class="sxs-lookup"><span data-stu-id="156f1-151">Request</span></span>
<span data-ttu-id="156f1-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="156f1-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="156f1-153">応答</span><span class="sxs-lookup"><span data-stu-id="156f1-153">Response</span></span>
<span data-ttu-id="156f1-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="156f1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




