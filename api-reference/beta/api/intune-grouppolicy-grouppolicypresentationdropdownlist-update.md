---
title: grouppolicypresentationdropdownlist の更新
description: grouppolicypresentationdropdownlist オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 170034d102f0d03bad1ca35e36f1d8219ab249ba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989060"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="a3e1e-103">grouppolicypresentationdropdownlist の更新</span><span class="sxs-lookup"><span data-stu-id="a3e1e-103">Update groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="a3e1e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3e1e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3e1e-106">[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-106">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3e1e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3e1e-107">Prerequisites</span></span>
<span data-ttu-id="a3e1e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3e1e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3e1e-110">Permission type</span></span>|<span data-ttu-id="a3e1e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3e1e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3e1e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3e1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3e1e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3e1e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a3e1e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3e1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3e1e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-115">Not supported.</span></span>|
|<span data-ttu-id="a3e1e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3e1e-116">Application</span></span>|<span data-ttu-id="a3e1e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3e1e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3e1e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="a3e1e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3e1e-119">Request headers</span></span>
|<span data-ttu-id="a3e1e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3e1e-120">Header</span></span>|<span data-ttu-id="a3e1e-121">値</span><span class="sxs-lookup"><span data-stu-id="a3e1e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3e1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3e1e-122">Authorization</span></span>|<span data-ttu-id="a3e1e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3e1e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a3e1e-124">Accept</span></span>|<span data-ttu-id="a3e1e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3e1e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3e1e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3e1e-126">Request body</span></span>
<span data-ttu-id="a3e1e-127">要求本文で、 [grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="a3e1e-128">次の表に、 [grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="a3e1e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3e1e-129">Property</span></span>|<span data-ttu-id="a3e1e-130">型</span><span class="sxs-lookup"><span data-stu-id="a3e1e-130">Type</span></span>|<span data-ttu-id="a3e1e-131">説明</span><span class="sxs-lookup"><span data-stu-id="a3e1e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e1e-132">label</span><span class="sxs-lookup"><span data-stu-id="a3e1e-132">label</span></span>|<span data-ttu-id="a3e1e-133">String</span><span class="sxs-lookup"><span data-stu-id="a3e1e-133">String</span></span>|<span data-ttu-id="a3e1e-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a3e1e-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-135">The default value is empty.</span></span> <span data-ttu-id="a3e1e-136">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a3e1e-137">id</span><span class="sxs-lookup"><span data-stu-id="a3e1e-137">id</span></span>|<span data-ttu-id="a3e1e-138">String</span><span class="sxs-lookup"><span data-stu-id="a3e1e-138">String</span></span>|<span data-ttu-id="a3e1e-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-139">Key of the entity.</span></span> <span data-ttu-id="a3e1e-140">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a3e1e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3e1e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a3e1e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3e1e-142">DateTimeOffset</span></span>|<span data-ttu-id="a3e1e-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="a3e1e-144">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a3e1e-145">defaultitem</span><span class="sxs-lookup"><span data-stu-id="a3e1e-145">defaultItem</span></span>|[<span data-ttu-id="a3e1e-146">grouppolicypresentationdropdownlistitem</span><span class="sxs-lookup"><span data-stu-id="a3e1e-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="a3e1e-147">アイテムのリストの既定の選択を示すローカライズされた文字列値。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="a3e1e-148">items</span><span class="sxs-lookup"><span data-stu-id="a3e1e-148">items</span></span>|<span data-ttu-id="a3e1e-149">[grouppolicypresentationdropdownlistitem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a3e1e-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="a3e1e-150">ローカライズされた表示名とそれに関連する値のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="a3e1e-151">必須</span><span class="sxs-lookup"><span data-stu-id="a3e1e-151">required</span></span>|<span data-ttu-id="a3e1e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3e1e-152">Boolean</span></span>|<span data-ttu-id="a3e1e-153">[パラメーター] ボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="a3e1e-154">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="a3e1e-155">応答</span><span class="sxs-lookup"><span data-stu-id="a3e1e-155">Response</span></span>
<span data-ttu-id="a3e1e-156">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-156">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3e1e-157">例</span><span class="sxs-lookup"><span data-stu-id="a3e1e-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3e1e-158">要求</span><span class="sxs-lookup"><span data-stu-id="a3e1e-158">Request</span></span>
<span data-ttu-id="a3e1e-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```

### <a name="response"></a><span data-ttu-id="a3e1e-160">応答</span><span class="sxs-lookup"><span data-stu-id="a3e1e-160">Response</span></span>
<span data-ttu-id="a3e1e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3e1e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```




