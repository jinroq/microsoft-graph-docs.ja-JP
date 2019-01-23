---
title: GroupPolicyPresentationValueLongDecimal を更新します。
description: GroupPolicyPresentationValueLongDecimal オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3aa3ad13f449bb8671688b94c5fb2530207fd2bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430438"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="bf15d-103">GroupPolicyPresentationValueLongDecimal を更新します。</span><span class="sxs-lookup"><span data-stu-id="bf15d-103">Update groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="bf15d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf15d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf15d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf15d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf15d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf15d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf15d-107">[GroupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bf15d-107">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf15d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bf15d-108">Prerequisites</span></span>
<span data-ttu-id="bf15d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf15d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bf15d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf15d-111">Permission type</span></span>|<span data-ttu-id="bf15d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf15d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf15d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bf15d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf15d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf15d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf15d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf15d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf15d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf15d-116">Not supported.</span></span>|
|<span data-ttu-id="bf15d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf15d-117">Application</span></span>|<span data-ttu-id="bf15d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf15d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf15d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf15d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="bf15d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf15d-120">Request headers</span></span>
|<span data-ttu-id="bf15d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf15d-121">Header</span></span>|<span data-ttu-id="bf15d-122">値</span><span class="sxs-lookup"><span data-stu-id="bf15d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf15d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf15d-123">Authorization</span></span>|<span data-ttu-id="bf15d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bf15d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf15d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf15d-125">Accept</span></span>|<span data-ttu-id="bf15d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf15d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf15d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf15d-127">Request body</span></span>
<span data-ttu-id="bf15d-128">要求の本文に[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="bf15d-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="bf15d-129">[GroupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="bf15d-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="bf15d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf15d-130">Property</span></span>|<span data-ttu-id="bf15d-131">型</span><span class="sxs-lookup"><span data-stu-id="bf15d-131">Type</span></span>|<span data-ttu-id="bf15d-132">説明</span><span class="sxs-lookup"><span data-stu-id="bf15d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf15d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf15d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="bf15d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf15d-134">DateTimeOffset</span></span>|<span data-ttu-id="bf15d-135">日付と時刻オブジェクトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="bf15d-135">The date and time the object was last modified.</span></span> <span data-ttu-id="bf15d-136">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bf15d-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="bf15d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf15d-137">createdDateTime</span></span>|<span data-ttu-id="bf15d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf15d-138">DateTimeOffset</span></span>|<span data-ttu-id="bf15d-139">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bf15d-139">The date and time the object was created.</span></span> <span data-ttu-id="bf15d-140">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bf15d-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="bf15d-141">id</span><span class="sxs-lookup"><span data-stu-id="bf15d-141">id</span></span>|<span data-ttu-id="bf15d-142">String</span><span class="sxs-lookup"><span data-stu-id="bf15d-142">String</span></span>|<span data-ttu-id="bf15d-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bf15d-143">Key of the entity.</span></span> <span data-ttu-id="bf15d-144">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bf15d-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="bf15d-145">value</span><span class="sxs-lookup"><span data-stu-id="bf15d-145">value</span></span>|<span data-ttu-id="bf15d-146">Int64</span><span class="sxs-lookup"><span data-stu-id="bf15d-146">Int64</span></span>|<span data-ttu-id="bf15d-147">関連付けられているプレゼンテーションの符号なし long 値。</span><span class="sxs-lookup"><span data-stu-id="bf15d-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="bf15d-148">応答</span><span class="sxs-lookup"><span data-stu-id="bf15d-148">Response</span></span>
<span data-ttu-id="bf15d-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bf15d-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf15d-150">例</span><span class="sxs-lookup"><span data-stu-id="bf15d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf15d-151">要求</span><span class="sxs-lookup"><span data-stu-id="bf15d-151">Request</span></span>
<span data-ttu-id="bf15d-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bf15d-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="bf15d-153">応答</span><span class="sxs-lookup"><span data-stu-id="bf15d-153">Response</span></span>
<span data-ttu-id="bf15d-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bf15d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```




