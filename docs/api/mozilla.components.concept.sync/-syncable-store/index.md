[android-components](../../index.md) / [mozilla.components.concept.sync](../index.md) / [SyncableStore](./index.md)

# SyncableStore

`interface SyncableStore` [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/concept/sync/src/main/java/mozilla/components/concept/sync/Sync.kt#L62)

Describes a "sync" entry point for a storage layer.

### Functions

| Name | Summary |
|---|---|
| [getHandle](get-handle.md) | `abstract fun getHandle(): `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)<br>This should be removed. See: https://github.com/mozilla/application-services/issues/1877 |

### Extension Functions

| Name | Summary |
|---|---|
| [loadResourceAsString](../../mozilla.components.support.test.file/kotlin.-any/load-resource-as-string.md) | `fun `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`.loadResourceAsString(path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Loads a file from the resources folder and returns its content as a string object. |

### Inheritors

| Name | Summary |
|---|---|
| [LockableStore](../-lockable-store/index.md) | `interface LockableStore : `[`SyncableStore`](./index.md)<br>An extension of [SyncableStore](./index.md) that can be locked/unlocked using an encryption key. |
| [PlacesBookmarksStorage](../../mozilla.components.browser.storage.sync/-places-bookmarks-storage/index.md) | `open class PlacesBookmarksStorage : `[`PlacesStorage`](../../mozilla.components.browser.storage.sync/-places-storage/index.md)`, `[`BookmarksStorage`](../../mozilla.components.concept.storage/-bookmarks-storage/index.md)`, `[`SyncableStore`](./index.md)<br>Implementation of the [BookmarksStorage](../../mozilla.components.concept.storage/-bookmarks-storage/index.md) which is backed by a Rust Places lib via [PlacesApi](#). |
| [PlacesHistoryStorage](../../mozilla.components.browser.storage.sync/-places-history-storage/index.md) | `open class PlacesHistoryStorage : `[`PlacesStorage`](../../mozilla.components.browser.storage.sync/-places-storage/index.md)`, `[`HistoryStorage`](../../mozilla.components.concept.storage/-history-storage/index.md)`, `[`SyncableStore`](./index.md)<br>Implementation of the [HistoryStorage](../../mozilla.components.concept.storage/-history-storage/index.md) which is backed by a Rust Places lib via [PlacesApi](#). |
| [PlacesStorage](../../mozilla.components.browser.storage.sync/-places-storage/index.md) | `abstract class PlacesStorage : `[`Storage`](../../mozilla.components.concept.storage/-storage/index.md)`, `[`SyncableStore`](./index.md)<br>A base class for concrete implementations of PlacesStorages |
| [RemoteTabsStorage](../../mozilla.components.browser.storage.sync/-remote-tabs-storage/index.md) | `open class RemoteTabsStorage : `[`Storage`](../../mozilla.components.concept.storage/-storage/index.md)`, `[`SyncableStore`](./index.md)<br>An interface which defines read/write methods for remote tabs data. |
