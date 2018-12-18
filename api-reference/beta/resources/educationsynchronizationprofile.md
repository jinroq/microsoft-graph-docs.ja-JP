---
title: educationSynchronizationProfile リソースの種類
description: 教育エンティティと、ソース ディレクトリから Azure Active directory (AD の Azure) の名簿の情報を同期するために使用する構成のセットを表します。 このリソースは、学校のデータの同期で使用されるプログラムの表現を提供します。
author: mmast-msft
ms.openlocfilehash: 43cf3ebd882c1e2dd86ada5621abbcd28b0e84c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363740"
---
# <a name="educationsynchronizationprofile-resource-type"></a>educationSynchronizationProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

教育エンティティと、ソース ディレクトリから Azure Active directory (AD の Azure) の名簿の情報を同期するために使用する構成のセットを表します。 このリソースは、[学校のデータの同期](https://sds.microsoft.com)で使用されるプログラムの表現を提供します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期プロファイルのリスト](../api/educationsynchronizationprofile-list.md) | **educationSynchronizationProfile**コレクション | テナント内のすべての同期プロファイルの一覧を取得します。 |
| [同期プロファイルを取得します。](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | プロファイル識別子を指定した特定のプロファイルを取得します。 |
| [同期プロファイルを作成します。](../api/educationsynchronizationprofile-post.md) | なし | 新しい同期プロファイルを作成します。 |
| [同期プロファイルを削除します。](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | プロファイル識別子を指定した特定のプロファイルを削除します。 |
| [進行中の同期を一時停止します。](../api/educationsynchronizationprofile-pause.md) | なし | 実行中の同期を一時停止します。 |
| [一時停止中の同期を再開します。](../api/educationsynchronizationprofile-resume.md) | なし | 一時停止中の同期を再開します。 |
| [同期をリセットします。](../api/educationsynchronizationprofile-reset.md) | なし | プロファイルの状態をリセットし、同期を再開します。 |
| [アップロードされたファイルの同期を開始します。](../api/educationsynchronizationprofile-start.md) | [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)コレクション| アップロードされたソース ファイルを確認し、同期を開始します。 データ プロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)が場合にのみ適用されます。 |
| [アップロード先の URL を取得します。](../api/educationsynchronizationprofile-uploadurl.md) | string | CSV データ ファイルをアップロードするのには短時間の URL を返します。 データ プロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)が場合にのみ適用されます。 |
| [同期のステータスを取得します。](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | 特定の同期プロファイルの状態を返します。 |
| [同期エラーが発生をします。](../api/educationsynchronizationerrors-get.md) | [educationSynchronizationError](educationsynchronizationerror.md)コレクション| 同期処理中に生成されたすべてのエラーを取得します。 |

## <a name="properties"></a>Properties

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **displayName** | string |  アイデンティティの同期の構成プロファイルの名前。         |
| **データプロバイダー** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  プロファイルに使用するデータ プロバイダーです。         |
| **identitysynchronizationconfiguration** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | アイデンティティの[作成](educationidentitycreationconfiguration.md)時または[一致する](educationidentitymatchingconfiguration.md)構成です。        |
| **licensesToAssign** | [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)コレクション|  セットアップ構成を使用します。        |
| **state** | string |  プロファイルの状態です。 可能な値は、`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed` です。          |

## <a name="relationships"></a>リレーションシップ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **errors** | [educationSynchronizationError](educationsynchronizationerror.md)コレクション| この同期プロファイルに関連付けられているすべてのエラー。 |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | 同期の状態です。 |

## <a name="json-representation"></a>JSON 表記
**EducationSynchronizationProfile**リソースの JSON の形式を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "#microsoft.graph.educationcsvdataprovider" },
    "identitySynchronizationConfiguration": { "@odata.type": "#microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
