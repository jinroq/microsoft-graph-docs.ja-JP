---
title: GroupPolicyPresentationValueText を更新します。
description: GroupPolicyPresentationValueText オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f0a1222c9abac4cbc459f25444e3cb37d6576a7e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430466"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="83e0c-103">GroupPolicyPresentationValueText を更新します。</span><span class="sxs-lookup"><span data-stu-id="83e0c-103">Update groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="83e0c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83e0c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83e0c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83e0c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83e0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83e0c-107">[GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="83e0c-107">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83e0c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="83e0c-108">Prerequisites</span></span>
<span data-ttu-id="83e0c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83e0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83e0c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83e0c-111">Permission type</span></span>|<span data-ttu-id="83e0c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="83e0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83e0c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83e0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83e0c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e0c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="83e0c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83e0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83e0c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e0c-116">Not supported.</span></span>|
|<span data-ttu-id="83e0c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83e0c-117">Application</span></span>|<span data-ttu-id="83e0c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83e0c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83e0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="83e0c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83e0c-120">Request headers</span></span>
|<span data-ttu-id="83e0c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83e0c-121">Header</span></span>|<span data-ttu-id="83e0c-122">値</span><span class="sxs-lookup"><span data-stu-id="83e0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83e0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83e0c-123">Authorization</span></span>|<span data-ttu-id="83e0c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="83e0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83e0c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83e0c-125">Accept</span></span>|<span data-ttu-id="83e0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83e0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83e0c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="83e0c-127">Request body</span></span>
<span data-ttu-id="83e0c-128">要求の本文に[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="83e0c-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="83e0c-129">[GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="83e0c-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="83e0c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83e0c-130">Property</span></span>|<span data-ttu-id="83e0c-131">型</span><span class="sxs-lookup"><span data-stu-id="83e0c-131">Type</span></span>|<span data-ttu-id="83e0c-132">説明</span><span class="sxs-lookup"><span data-stu-id="83e0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83e0c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83e0c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="83e0c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83e0c-134">DateTimeOffset</span></span>|<span data-ttu-id="83e0c-135">日付と時刻オブジェクトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="83e0c-135">The date and time the object was last modified.</span></span> <span data-ttu-id="83e0c-136">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="83e0c-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="83e0c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83e0c-137">createdDateTime</span></span>|<span data-ttu-id="83e0c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83e0c-138">DateTimeOffset</span></span>|<span data-ttu-id="83e0c-139">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="83e0c-139">The date and time the object was created.</span></span> <span data-ttu-id="83e0c-140">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="83e0c-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="83e0c-141">id</span><span class="sxs-lookup"><span data-stu-id="83e0c-141">id</span></span>|<span data-ttu-id="83e0c-142">String</span><span class="sxs-lookup"><span data-stu-id="83e0c-142">String</span></span>|<span data-ttu-id="83e0c-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="83e0c-143">Key of the entity.</span></span> <span data-ttu-id="83e0c-144">[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="83e0c-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="83e0c-145">value</span><span class="sxs-lookup"><span data-stu-id="83e0c-145">value</span></span>|<span data-ttu-id="83e0c-146">文字列</span><span class="sxs-lookup"><span data-stu-id="83e0c-146">String</span></span>|<span data-ttu-id="83e0c-147">関連付けられているプレゼンテーションの文字列値。</span><span class="sxs-lookup"><span data-stu-id="83e0c-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="83e0c-148">応答</span><span class="sxs-lookup"><span data-stu-id="83e0c-148">Response</span></span>
<span data-ttu-id="83e0c-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="83e0c-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83e0c-150">例</span><span class="sxs-lookup"><span data-stu-id="83e0c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="83e0c-151">要求</span><span class="sxs-lookup"><span data-stu-id="83e0c-151">Request</span></span>
<span data-ttu-id="83e0c-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83e0c-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="83e0c-153">応答</span><span class="sxs-lookup"><span data-stu-id="83e0c-153">Response</span></span>
<span data-ttu-id="83e0c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83e0c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




